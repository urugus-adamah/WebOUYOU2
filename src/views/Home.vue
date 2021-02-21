<template>
  <div class="flex">
    <div class="left">
      <SideNavi />
    </div>
    <div class="right">
      <p class="title">ホーム</p>
      <Message />
    </div>
  </div>

</template>
<script>
import SideNavi from "../components/SideNavi";
import Message from "../components/Message";
export default {
  components:{
    SideNavi,
    Message
  }
};
</script>
<style scoped>
  .flex{
    display: flex;
  }
  .left{
    width:25%
  }
  .right{
    width: 75%;
  }
  .title{
      padding: 10px 0;
      border: solid 1px white;
  }
</style>