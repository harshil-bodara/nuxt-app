<template>
     <form @click="onSave">
                <AppcontrolInput v-model="editpost.author">Author Name</AppcontrolInput>
                <AppcontrolInput v-model="editpost.title">Title</AppcontrolInput>
                <AppcontrolInput v-model="editpost.thumbnaillink">Thumbnail Link</AppcontrolInput>
                <AppcontrolInput control-type="textarea" v-model="editpost.content">Content</AppcontrolInput>
                <Appbutton type="submit">Save</Appbutton>
                <Appbutton type="button" style="margin-left:10px;background:red;" btn-style="cencel" @click="onCancel">Cancel</Appbutton>
            </form>
</template>

<script>
import AppcontrolInput from '@/components/ui/appcontrollput.vue'
import AppButton from '@/components/ui/appbutton.vue'

export default {
    components:{
        AppButton,
        AppcontrolInput
    },
    props:{
        post:{
            type:Object,
            required:false
        }
    },
    data(){
        return {
            editpost: this.post ? {...this.post} : {
                author:'',
                title:'',
                thumbnaillink:'',
                content:''               
            }
        }
    },
    methods:{
        onSave(){
            console.log("this.editpost",this.editpost)
        },
        onCancel(){
            this.$router.push('/admin');
        }
    }
}
</script>