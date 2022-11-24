<template>
    <main>
        <div class="cont-1">
            <div class="content">
              <h2> <i class="fa-solid fa-arrow-right"></i> Content goes here <i class="fa-solid fa-arrow-left"></i> </h2> 
            </div> 
        </div>
        <div class="cont-2">
            <div class="immagini">
                <div class="img-text">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="img1">
                    <span>DIGITAL COMICS</span>
                </div>
                <div class="img-text">
                    <img src="../assets/img/buy-comics-merchandise.png" alt="img2">
                    <span>DC MERCHANDISE</span>
                </div>
                <div class="img-text">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="img3">
                    <span>SUBSCRIPTION</span>
                </div>
                <div class="img-text">
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="img4">
                    <span>COMIC SHOP LOCATOR</span>
                </div>
                <div class="img-text">
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="img5">
                    <span>DC POWER VISA</span>
                </div>               
            </div>
        </div>
    </main>
</template>

<script>
export default {
  name: 'MainComp',
}
</script>

<style lang="scss">

main{
    color: white;
}

.cont-1{
    background-color: rgb(0, 0, 0, 0.9);
    height: 15vh;  
    display: flex;
}

.content{
    display: flex;
    align-items: center;
    justify-content: flex-start;
    width: 80%;
    margin: auto;
}

.cont-2{
    background-color: dodgerblue;
    height: 15vh;  
}

.immagini{
    display: flex;
    justify-content: center;
    padding: 30px 0;
    gap: 4rem;
}

.immagini img{
    height: 45px;
}

.img-text{
    display: flex;
    align-items: center;
    font-size: 13px;
    gap: 10px;
}


</style>