<template>
        <div class="Hoke">
            <h2>{{title}}</h2>
        <button @click="changeTitle">Update</button>
        </div>
</template>


<script>
export default {
   name:'Hoke',
   data(){
       return{
        title:'Hoke Part'
       }
   },
   methods:{
       changeTitle(){
           this.title = 'openjanala IT'
       }
   },
    beforeCreate(){
//alert('beforeCreate')
    },
    created(){
//alert('created')
    },
    beforeUpdate(){
        alert('befor update')
    },
    updated(){
        alert('updated')
    },
}
</script>


<style scoped>

</style>