<template>
    <div class="admin-post-page">
        <section class="update-form">
            <AdminPostForm :post="loadedpost"/>
        </section>
    </div>
</template>

<script>
import AdminPostForm from '~/components/admin/adminpost.vue';

export default {
    components:{
        AdminPostForm
    },
    data(){
        return{
            loadedpost:{
                author:"test",
                title:"tester",
                content:"hello world",
                thumbnaillink:"http://helloworld.com"
            }
        }
    }
}
</script>