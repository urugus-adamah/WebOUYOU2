<template>
  <div class="home">
    <div class="side-nav">
      <img class="logo" alt="Vue logo" src="../assets/logo.png">
      <div>
        <ul>
          <li class="home" @click="$router.push('/home')">
            <img src="../assets/home.png" alt="">
             ホーム
          </li>
          <li class="profile" @click="$router.push('/profile')">
              <img src="../assets/profile.png" alt="">
              プロフィール
            </li>
          <li class="logout" @click="$router.push('/')">
            <img src="../assets/logout.png" alt="">
            ログアウト
          </li>
        </ul>
      </div>
      <ShareMessage/>
    </div>
  </div>
</template>

<script>
  import ShareMessage from "../components/ShareMessage"
export default {
  components:{
    ShareMessage
  }
};
</script>
<style scoped>
  .side-nav{
    padding: 20px;
    width:250px;
  }
  .logo{
    width: 150px;
    cursor: pointer;
  }
  li{
    margin-top: 15px;
    list-style: none;
    cursor:pointer;
  }
  ul img{
    width: 20px;
    margin-right: 20px;
  }
</style>
