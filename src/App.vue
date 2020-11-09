<template>
  <div id="app">
    <!-- Header -->
    <header id="header">
      <h1><a href="index.html">Future Imperfect</a></h1>
      <nav class="links">
        <ul>
          <li><a href="/">Home</a></li>
          <li><a href="/posts">Posts</a></li>
          <li><a href="/signup">Signup</a></li>
          <li><a href="/login">Login</a></li>
          <li><a href="/logout">Logout</a></li>
        </ul>
      </nav>
      <nav class="main">
        <ul>
          <li class="search">
            <a class="fa-search" href="#search">Search</a>
            <form id="search" method="get" action="#">
              <input type="text" name="query" placeholder="Search" />
            </form>
          </li>
          <li class="menu">
            <a class="fa-bars" href="#menu">Menu</a>
          </li>
        </ul>
      </nav>
    </header>
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/posts">All posts</router-link> |
      <router-link to="/signup">Signup</router-link> |
      <router-link to="/login">Login</router-link> |
      <router-link to="/logout">Logout</router-link> |
      <router-link to="/posts/new">New post</router-link>
    </div> -->

    <router-view/>

    <!-- Footer -->
    <section id="footer">
      <ul class="icons">
        <li><a href="#" class="icon brands fa-twitter"><span class="label">Twitter</span></a></li>
        <li><a href="#" class="icon brands fa-facebook-f"><span class="label">Facebook</span></a></li>
        <li><a href="#" class="icon brands fa-instagram"><span class="label">Instagram</span></a></li>
        <li><a href="#" class="icon solid fa-rss"><span class="label">RSS</span></a></li>
        <li><a href="#" class="icon solid fa-envelope"><span class="label">Email</span></a></li>
      </ul>
      <p class="copyright">&copy; Untitled. Design: <a href="http://html5up.net">HTML5 UP</a>. Images: <a href="http://unsplash.com">Unsplash</a>.</p>
    </section>
  </div>
</template>

<style>
</style>
