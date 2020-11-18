<template>
  <div v-bind:id="$route.name === 'posts-index' ? 'wrapper' : 'app'">
    <!-- Header -->
    <header id="header">
      <h1><a href="/">Serenity</a></h1>
      <nav class="links">
        <ul>
          <li><a href="/posts">Posts</a></li>
          <li><a href="/signup">Signup</a></li>
          <li><a href="/login">Login</a></li>
          <li><a href="/logout">Logout</a></li>
          <li><a href="/webcamExample">Webcam Example</a></li>
          <li><a href="/posts/new">Create Post</a></li>
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
<!-- Sidebar -->
					<section id="sidebar" v-if="$route.name==='posts-index'">

						<!-- Intro -->
							<section id="intro">
								<a href="#" class="logo"><img src="https://images.unsplash.com/photo-1495211895963-08d8812dcbf0?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80" alt="" /></a>
								<header>
									<h2>Kirill Grinash</h2>
									<p>Juniors Data Information</p>
								</header>
							</section>

						<!-- Mini Posts -->
							<section>
								<div class="mini-posts">

									<!-- Mini Post -->
										<article class="mini-post">
											<header>
												<h3><a href="single.html">Bobby Grinash</a></h3>
												
											</header>
											<a href="single.html" class="image"><img src="images/pic04.jpg" alt="" /></a>
										</article>

									<!-- Mini Post -->
										<article class="mini-post">
											<header>
												<h3><a href="single.html">Daisy Grinash</a></h3>
												
											</header>
											<a href="single.html" class="image"><img src="images/pic05.jpg" alt="" /></a>
										</article>

									<!-- Mini Post -->
										<article class="mini-post">
											<header>
												<h3><a href="single.html">Oliver Grinash</a></h3>
												
											</header>
											<a href="single.html" class="image"><img src="images/pic06.jpg" alt="" /></a>
										</article>

								</div>
							</section>

						<!-- Posts List -->
							<!-- <section>
								<ul class="posts">
									<li>
										<article>
											<header>
												<h3><a href="single.html">Lorem ipsum fermentum ut nisl vitae</a></h3>
												<time class="published" datetime="2015-10-20">October 20, 2015</time>
											</header>
											<a href="single.html" class="image"><img src="images/pic08.jpg" alt="" /></a>
										</article>
									</li>
									<li>
										<article>
											<header>
												<h3><a href="single.html">Convallis maximus nisl mattis nunc id lorem</a></h3>
												<time class="published" datetime="2015-10-15">October 15, 2015</time>
											</header>
											<a href="single.html" class="image"><img src="images/pic09.jpg" alt="" /></a>
										</article>
									</li>
									<li>
										<article>
											<header>
												<h3><a href="single.html">Euismod amet placerat vivamus porttitor</a></h3>
												<time class="published" datetime="2015-10-10">October 10, 2015</time>
											</header>
											<a href="single.html" class="image"><img src="images/pic10.jpg" alt="" /></a>
										</article>
									</li>
									<li>
										<article>
											<header>
												<h3><a href="single.html">Magna enim accumsan tortor cursus ultricies</a></h3>
												<time class="published" datetime="2015-10-08">October 8, 2015</time>
											</header>
											<a href="single.html" class="image"><img src="images/pic11.jpg" alt="" /></a>
										</article>
									</li>
									<li>
										<article>
											<header>
												<h3><a href="single.html">Congue ullam corper lorem ipsum dolor</a></h3>
												<time class="published" datetime="2015-10-06">October 7, 2015</time>
											</header>
											<a href="single.html" class="image"><img src="images/pic12.jpg" alt="" /></a>
										</article>
									</li>
								</ul>
							</section> -->

						<!-- About -->
							<section class="blurb">
								<h2>About</h2>
								<p>Serenity is an app designed to give you an insight into how the computer affects your child’s emotional state. Serenity gives you direct feedback on the emotion your child exhibits during computer usage.</p>
								<ul class="actions">
									<li><a href="#" class="button">{{ message }}</a></li>
								</ul>
							</section>

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

					</section>
    
  </div>
</template>

<style>
</style>
<script>
export default {
  data: function () {
    return {
      message: "hello"
    }
  }
}
</script>
