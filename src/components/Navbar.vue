<template>
    <div>
        <nav>
            <ul>
                <li><a href="">Home</a></li>
                <li><a href="">Post</a></li>
                <li><a href="">About</a></li>
                <li><a href="">Contact</a></li>
            </ul>
        </nav>
    </div>
</template>

<script >
export default {
    name:'Navbar',
    data(){
        return{

        }
    }
}
</script>



<style scoped>
nav{
    text-align: center;
}
nav ul{
    padding:0;
}
nav li{
    display:inline-block;
    padding:20px 10px;
     
}
nav a {
    text-transform: uppercase;
    text-decoration: none;
}
</style>
