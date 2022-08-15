<template>
  <form action="">
    <input type="text" placeholder="title" v-model="title">
    <input type="text" placeholder="body" v-model="body">
    <button @click.prevent="sentData">submit</button>
  </form>
</template>

<script>
export default {
    data(){
        return {
            title: "",
            body: "",
        }
    },
    methods:{
        sentData(){
            this.$emit("sentData",{title:this.title,body:this.body})
        }
    }


}
</script>

<style>

</style>