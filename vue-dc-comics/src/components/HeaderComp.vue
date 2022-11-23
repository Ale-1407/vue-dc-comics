<template>
    <header>
        <img src="../assets/img/dc-logo.png" alt="logo" class="logo">
        <nav>
            <ul>
                <li>
                   <a href="#">CHARACTERS</a> 
                </li>
                <li>
                    <a href="#" class="active">COMICS</a> 
                </li>
                <li>
                   <a href="#">MOVIES</a> 
                </li>
                <li>
                   <a href="#">TV</a> 
                </li>
                <li>
                  <a href="#">GAMES</a>  
                </li>
                <li>
                   <a href="#">COLLECTIBLES</a> 
                </li>
                <li>
                   <a href="#">VIDEOS</a> 
                </li>
                <li>
                  <a href="#">FANS</a>  
                </li>
                <li>
                   <a href="#">NEWS</a> 
                </li>
                <li>
                   <a href="#">SHOP</a> 
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
  name: 'HeaderComp',
}
</script>

<style lang="scss">

header{
    padding: 15px 0;
    display: flex;
    justify-content: space-around;
}

nav{
    margin: auto 0;
}

ul{
  display: flex;
  align-items: center;

  li{
    padding: 10px;
    list-style-type: none;
    font-weight: bold;
    font-size: 13px;
  }
}

a{
    text-decoration: none;
    color: black;
}

.active{
    color: dodgerblue;
}


.logo{
    height: 80px;
}
</style>