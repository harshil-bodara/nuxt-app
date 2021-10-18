<template>
    <div class="admin-new-post-page">
        <section class="new-post-form">
          <AdminPostForm/>
        </section>
    </div>
</template>

<script>
import AdminPostForm from '~/components/admin/adminpost.vue';

export default {
    components:{
        AdminPostForm
    }
}
</script>

<style scoped>
.new-post-form{
    width: 90%;
    margin: 2px auto;
}
@media(min-width:768px) {
    .new-post-form{
        width: 500px;
    }
}
</style>