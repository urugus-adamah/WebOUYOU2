<template>
  <div class="header flex">
    <div class="left">
      <img class="logo" src="../assets/logo.png" alt="" @click="$router.push('/')">
    </div>
    <div class="right flex">
      <p @click="$router.push('/signup')">新規登録</p>
      <p @click="$router.push('/')">ログイン</p>
    </div>
  </div>
</template>

<style scoped>
.header{
    justify-content: space-between;
    margin: 20px;
  }
  .logo{
    width: 150px;
    cursor: pointer;
  }
  .flex{
    display: flex;
    justify-content: space-between;
  }
  .right p{
    margin-right: 20px;
    cursor: pointer;
  }
</style>