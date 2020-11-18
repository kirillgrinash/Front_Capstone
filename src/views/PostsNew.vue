<template>
  <div id="post_new">
    <div class="posts-new">
      <h1>New Post</h1>
      <form v-on:submit.prevent="createPost()">
        <ul>
          <li v-for="error in errors">{{ error }}</li>
        </ul>
        Name: <input type="text" v-model="newPostName" />
        Body: <input type="text" v-model="newPostBody" />
        Image: <input type="text" v-model="newPostImage" />
        <input type="submit" value="Create" />
      </form>
    </div>
  </div>
</template>

<style>
#post_new {
      margin: 0;
      padding: 0;
      width: 100vw;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    canvas {
      position: absolute;
    }
</style>

<script>
import axios from "axios";
export default {
  data: function() {
    return {
      newPostName: "",
      newPostBody: "",
      newPostImage: "",
      errors: [],
    };
  },
  created: function() {},
  methods: {
    createPost: function() {
      var params = {
        name: this.newPostName,
        body: this.newPostBody,
        image: this.newPostImage,
      };
      axios
        .post("/api/posts", params)
        .then(response => {
          console.log("posts create", response);
          this.$router.push("/posts");
        })
        .catch(error => {
          console.log("posts create error", error.response);
          this.errors = error.response.data.errors;
        });
    },
  },
};
</script>