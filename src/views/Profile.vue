<template>
  <div class="flex">
    <div class="left">
      <SideNavi />
    </div>
    <div class="right">
      <p class="title">プロフィール</p>
      <div class="profile-box">
        <div class="flex profile-head">
          <p :class="name">{{name}}</p>
          <button>変更する</button>
        </div>
        <p class="profile" :class="profile">{{profile}}</p>
      </div>
      <Message />
    </div>
  </div>
</template>
<script>
import SideNavi from "../components/SideNavi";
import Message from "../components/Message";
export default {
  data(){
    return{
      name:"test",
      profile:"testtest"
    };
  },
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
  .profile-box{
    justify-content: space-between;
    padding: 20px 10px;
    border: solid 1px white;
  }
  .profile-head{
    justify-content: space-between;
    vertical-align: top;
  }
  .profile{
    font-size: 0.8em;
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
    button{
    /* margin-top: 10px; */
    border-radius: 20px;
    background-color: purple;
    cursor: pointer;
  }
</style>