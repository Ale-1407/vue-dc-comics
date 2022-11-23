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
    background-color: black;
    height: 130px;  
    display: flex;
}

.content{
    align-self: center;
    text-align: left;
    margin-left: 8rem;
}

.cont-2{
    background-color: dodgerblue;
    height: 140px;  

}

.immagini{
    display: flex;
    justify-content: space-around;
    padding: 40px 0;
}

.immagini img{
    height: 55px;
}

.img-text{
    display: flex;
    align-items: center;
    font-size: 13px;
    gap: 10px;
}


</style>