<template>
  <div>
    <HeaderAuth/>
    <div class="card">
      <p>新規登録</p>
      <div class="form">
        <input type="text"  placeholder="ユーザーネーム">
        <input type="text" placeholder="プロフィール">
        <input type="email" placeholder="メールアドレス">
        <input type="password" placeholder="パスワード">
        <button>新規登録</button>
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
</style>