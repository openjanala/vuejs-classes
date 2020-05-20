<template>
  <div id="app">
    <h2>{{ title }}</h2>
    <Navbar></Navbar>
    <Hoke></Hoke>

    <Footer></Footer>
  </div>
</template>


<script>
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'
import Hoke from './components/Hoke.vue'



export default {
  name: 'app',
  data(){
    return{
      title:'Hurray! our vue apps are running:)',
    
    }
  },
  components:{
  Navbar,
  Footer,
  Hoke

  },
  methods:{

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
