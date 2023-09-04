<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <div>
    <h4>더 원룸</h4>
    <p>{{price1}}만원</p> 
  </div>
  <div>
    <h4>숭이 원룸</h4>
    <p>{{price2}}만원</p>
  </div>
</template>

<script>

export default {
  name: 'App',
  data(){ //데이터 보관함 모두 여기 저장
    return {
      price1 : 60,
      price2 : 80,
      products : ['역삼동원룸', '천호동원룸' , ' 마포구원룸']

    }
  },
  components: {

  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
