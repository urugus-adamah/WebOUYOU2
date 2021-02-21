<template>
  <div class="share">
        <p>シェア</p>
        <textarea ></textarea>
        <div class="btn-share">
          <button>シェアする</button>
        </div>
    </div>
</template>
<style scoped>
  .share{
    margin-top: 20px;
  }
  .btn-share{
    text-align: right;
  }
  .btn-share button{
    margin-top: 10px;
    border-radius: 20px;
    background-color: purple;
    cursor: pointer;
  }
  textarea{
    margin-top: 10px;
    width: 100%;
    height: 100px;
    border-radius: 5px;
    background-color: black;
  }
</style>