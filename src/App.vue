<template>

  <div class = "menu">
    <a v-for="a in 메뉴들" :key="a"> {{a}}</a>

    
    
  </div>

  <div>
    <h4>{{ products[0] }}</h4>
    <p>50만원</p>
    <button @click="increase">허위매물신고</button> <span>신고수 : {{ 신고수 }}</span>
  </div>
  <div>
    <h4>{{ products[1] }} 원룸</h4>
    <p>60만원</p>
  </div>
  <div>
    <h4>{{ products[2] }}원룸</h4>
    <p>70만원</p>
  </div>
</template>

<script>


export default {
  name: 'App',
  data(){ //데이터 보관함 모두 여기 저장
    return {
      신고수 : 0,
      메뉴들 : ['Home', 'Shop', 'About'],
      products : ['역삼동원룸', '천호동원룸' , ' 마포구원룸']

    }
  },
  methods : {
    increase(){
      this.신고수 += 1;
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
  margin-top: 20px;
}

.menu {
  background: darkslateblue;
  padding: 15px;
  border-radius: 5px;
}
.menu a {
  color : white;
  padding : 10px;
}


</style>
