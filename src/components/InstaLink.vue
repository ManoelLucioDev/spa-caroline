<template>
    <div>
        <a href="" target="_blank" >
        <v-img 
            :width="width"
            :src= "require('@/assets/insta.png')"></v-img>
        </a>
    </div>
    
</template>


<script>
export default {
    name: 'InstaLink',
    data(){
        return{
            width: 65

        }
    }
}
</script>