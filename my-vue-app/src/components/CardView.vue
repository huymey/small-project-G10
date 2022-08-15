<template>
  <div class="card" v-for="(card,index) of postList" :key="index">
    <div class="card_title">{{card.title}}</div>
    <div class="card_body">{{card.body}}</div>
  </div>
</template>

<script>
export default {
    props:{
        postList:Array
    }
}
</script>

<style>
    .card {
        padding :10px;
        border-top: 5px solid rgb(7, 31, 252);
        border: 1px solid #000;
        margin: 5px;

    }
    .card_title {
        border-bottom: 1px solid rgb(7, 31, 252);
    }
</style>