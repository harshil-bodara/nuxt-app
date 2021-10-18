<template>
     <section class="post-list">
       <PostPreview 
          id="1"
          thumbnail="https://images.unsplash.com/photo-1634005083664-f06a3bbc9416?ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHw0fHx8ZW58MHx8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60"
          title="post 1"
          content="Hello world"
          />
       <PostPreview
          id="2"
          thumbnail="https://images.unsplash.com/photo-1634005083664-f06a3bbc9416?ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHw0fHx8ZW58MHx8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60"
          title="post 2"
          content="Hello world"
       />
      </section>
</template>

<script>
import PostPreview from '@/components/posts/postspreview.vue'

export default {
    components:{
        PostPreview
    }
}
</script>

<style scoped>
.post-list{
 display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>