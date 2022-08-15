<template>
  <Form @sentData="pushData"/>
  <Card :postList="cardList"/>
</template>

<script>
import Form from "./components/FormView.vue"
import Card from "./components/CardView.vue"
export default {
  components:{
    Form,Card
  },
  data(){
    return {
      cardList:[
        {title: "Hello guy",body:"I want to woo you. Are you ok?"},
        {title: "Hello guy",body:"I want to woo you. Are you ok?"},
        {title: "Hello guy",body:"I want to woo you. Are you ok?"},
      ]
    }
  },
  methods:{
    pushData(valueOb){
      this.cardList.push(valueOb);
    }
  }
}
</script>

<style>

</style>
