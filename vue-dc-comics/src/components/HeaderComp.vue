<template>
    <header>
        <img src="../assets/img/dc-logo.png" alt="logo" class="logo">
        <nav>
            <ul>
                <li>CHARACTERS</li>
                <li class="active">COMICS</li>
                <li>MOVIES</li>
                <li>TV</li>
                <li>GAMES</li>
                <li>COLLECTIBLES</li>
                <li>VIDEOS</li>
                <li>FANS</li>
                <li>NEWS</li>
                <li>SHOP</li>
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
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

header{
    padding: 10px 0;
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

.active{
    color: dodgerblue;   
}

.logo{
    height: 90px;
}
</style>