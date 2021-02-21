<template>
  <div>
    <HeaderAuth/>
    <div class="card">
      <p>ログイン</p>
      <div class="form">
        <input type="email"  placeholder="メールアドレス">
        <input type="password" placeholder="パスワード">
        <button @click="$router.push('/home')">ログイン</button>
      </div>
    </div>
  </div>
</template>

<script>
import HeaderAuth from "../components/HeaderAuth";
export default {
  components:{
    HeaderAuth
  }
};
</script>

<style scoped>
  input{
    margin-top: 10px;
    width: 80%;
    border-radius: 5px;
    color: black;
  }
  button{
    margin-top: 10px;
    border-radius: 20px;
    background-color: purple;
    cursor: pointer;
  }
  .card{
    margin: 100px auto;
    text-align: center;
    background-color: white;
    width: 300px;
    padding: 20px;
    /* height: 150px; */
    border-radius: 5px;
  }
  .card p{
    color: black;
    font-weight: bold;
  }

</style>