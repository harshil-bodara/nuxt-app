<template>
  <div class="home-page">
      <section class="intro">
        <h1>Get the latest tech news!</h1>
      </section>
      <section class="featured-posts">
        <nuxt-link :to="'/posts' +1">
          <article class="post-preview">
            <div class="post-preview"></div>
            <div class="post-thumbnail" style="background-image:url('https://images.unsplash.com/photo-1634005083664-f06a3bbc9416?ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHw0fHx8ZW58MHx8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60')"></div>
            <div class="post-content">
              <h2>Post title</h2>
               <p>Post content</p>
            </div>
          </article>
        </nuxt-link>
         <nuxt-link :to="'/posts' +1">
          <article class="post-preview">
            <div class="post-preview"></div>
            <div class="post-thumbnail" style="background-image:url('https://images.unsplash.com/photo-1634005083664-f06a3bbc9416?ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHw0fHx8ZW58MHx8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60')"></div>
            <div class="post-content">
              <h2>Post title</h2>
               <p>Post content</p>
            </div>
          </article>
        </nuxt-link>
         <nuxt-link :to="'/posts' +1">
          <article class="post-preview">
            <div class="post-preview"></div>
            <div class="post-thumbnail" style="background-image:url('https://images.unsplash.com/photo-1634005083664-f06a3bbc9416?ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHw0fHx8ZW58MHx8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60')"></div>
            <div class="post-content">
              <h2>Post title</h2>
               <p>Post content</p>
            </div>
          </article>
        </nuxt-link>
      </section>
  </div>
</template>

<style scoped>
.featured-posts{
  display: flex;
}
.post-preview{
 border: 1px solid #ccc;
 box-shadow: 0 2px 2px #ccc;
 background-color:#fff;
 width: 90%;
}

a{
  text-decoration: none;
  color:black
}

@media (min-width: 850px) {
  .post-preview{
    width: 400px;
    margin:10px;
  }
  .post-thumbnail{
    width: 100%;
    height: 200px;
    background-position: center;
    background-size: cover;
  }  
}
.post-content{
  padding: 10px;
  text-align: center;
}
a:hover .post-content,
a:active .post-content {
  background:#ccc;
}
</style>