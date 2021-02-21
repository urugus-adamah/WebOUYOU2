<template>
  <div >
    <div class="message-box"  v-for="(value,index) in shares"   :key="index">
      <div class="flex">
        <p class="name">{{value.name}}</p>
        <img class="icon" src="../assets/heart.png" alt="">
        <p>{{value.like.length}}</p>
        <img class="icon" src="../assets/cross.png" alt="">
        <img class="icon detail" src="../assets/detail.png" alt="">
      </div>
      <p class="message">{{value.share}}</p>
    </div>
  </div>
</template>
<script>
export default {
   data(){
    return{
      shares:[{name:"hama",like:[],share:"初めまして"}]
    }
  },
};
</script>
<style scoped>
  .flex{
    display: flex;  
  }

  .message-box{
    border: solid 1px white;
    padding: 10px;
    width: 100%;
    
  }
  .message{
    height: 50px;
    margin: 10px 0;
    width: 500px;
  }
  .name {
    text-align: left;
    /* width:50px; */
  }
  .icon{
    width: 20px;
    margin: 0 5px;
  }
  .detail{
    margin-left: 20px;
  }
</style>