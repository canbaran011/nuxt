<template>
    <div>
        <h1>    
            hey this is user page RIGHT?
        </h1>
        <input type="text" v-model="userId">
        <button
        @click="onLoadUser"
        >LoadUser</button>
        <nuxt-child/>
    </div>
</template>


<script>
export default {
    data(){
        return{
            userId:""
        }
    },
    methods: {
        onLoadUser(){
            this.$router.push("/users/"+ this.userId)
        }
    },
    layout : 'users'
    
}
</script>