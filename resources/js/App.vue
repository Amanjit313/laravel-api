<template>

</template>

<script>
export default {
    name: 'App',

    methods:{
        getApi(){
            axios.get('/api/posts')
            .then(response =>{
                console.log(response.data)
            })
        }
    },

    mounted(){
        this.getApi()
    }
}
</script>

<style>

</style>
