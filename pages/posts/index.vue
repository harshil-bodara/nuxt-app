<template>
    <div class="posts-page">    
        <PostList/>
    </div>
</template>

<script>
import PostList from '~/components/posts/postlist.vue'

export default {
    components:{
        PostList
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
.post-preview{
 border: 1px solid #ccc;
 box-shadow: 0 2px 2px #ccc;
 background-color:#fff;
 width: 90%;
}
.posts-page{
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>