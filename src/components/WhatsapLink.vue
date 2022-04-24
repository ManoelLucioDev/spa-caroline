<template>
    <div>
        <a href="https://web.whatsapp.com/send?phone=5521972000203" target="_blank" >
        <v-img 
            :width="width"
            :src= "require('@/assets/whatsap.png')"></v-img>
        </a>
    </div>
    
</template>


<script>
export default {
    name: 'WhatsapLink',
    data(){
        return{
            width: 35

        }
    }
}
</script>


