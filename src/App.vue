<template>
  <div id="app">
    <h2>{{ title }}</h2>
    <Navbar></Navbar>
    <AllFriends :friends="friends" @delete="deleteFriend"></AllFriends>
    <OnlineFriends :friends="friends"></OnlineFriends>
    <Footer></Footer>
  </div>
</template>


<script>
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'
import AllFriends from './components/AllFriends.vue'
import OnlineFriends from './components/OnlineFriends.vue'
export default {
  name: 'app',
  data(){
    return{
      title:'Hurray! our vue apps are running:)',
       friends:[
               {name:'A', online:true}, 
               {name:'B', online:true}, 
               {name:'C', online:false}, 
               {name:'D', online:false}, 
               {name:'E', online:true}
              
            ]
    }
  },
  components:{
Navbar,
Footer,
AllFriends,
OnlineFriends
  },
  methods:{
    deleteFriend(payload){
    //console.log(payload); 
    this.friends = this.friends.filter(friends=>{
      return friends.name !==payload.name
    })
    }
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
