<template>
    <main>
        <div class="cont-1">
            <div class="content"></div> 
        </div>
        <div class="cont-card">
          <button class="etichetta-blu">CURRENT SERIES</button>
          <div class="container-card">
            <CardComp v-for="(elem, index) in comics" :key="index" :dettagliComics="elem" />
          </div> 
          <div class="btn-comics">
            <button class="load-btn">LOAD MORE</button>
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

import CardComp from './CardComp.vue'

export default {
  name: 'MainComp',
  components: {
    CardComp
  },
  data(){
    return{
        comics: [
         {
           "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
           "price": "$19.99",
           "series": "Action Comics",
           "type": "comic book"
         },
         {
           "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
           "price": "$3.99",
           "series": "American Vampire 1976",
           "type": "comic book"
         },
         {
           "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
           "price": "$16.99",
           "series": "Aquaman",
           "type": "graphic novel"
         },
         {
           "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
           "price": "$2.99",
           "series": "Batgirl",
           "type": "comic book"
         },
         {
           "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
           "price": "$3.99",
           "series": "Batman",
           "type": "comic book"
         },
         {
           "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
           "price": "$2.99",
           "series": "Batman Beyond",
           "type": "comic book"
         },
         {
           "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
           "price": "$3.99",
           "series": "Batman/Superman",
           "type": "comic book"
         },
         {
           "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
           "price": "$4.99",
           "series": "Batman/Superman Annual",
           "type": "comic book"
         },
         {
           "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
           "price": "$5.99",
           "series": "Batman: The Joker War Zone",
           "type": "comic book"
         },
         {
           "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
           "price": "$6.99",
           "series": "Batman: Three Jokers",
           "type": "comic book"
         },
         {
           "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
           "price": "$4.99",
           "series": "Batman: White Knight Presents: Harley Quinn",
           "type": "comic book"
         },
         {
           "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
           "price": "$16.99",
           "series": "Catwoman",
           "type": "graphic novel"
         }
        ]
    }
  }
}
</script>

<style lang="scss">

main{
    color: white;
}

.cont-1{
    background-size: cover;
    background-image: url('../assets/img/jumbotron.jpg');
    height: 50vh;  
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
.img-text:hover{
  font-size: 15px;
  cursor: pointer;
}
.etichetta-blu{
  border: 1px solid transparent;
  background-color: dodgerblue;
  padding: 10px;
  color: white;
  position: relative;
  top: -25px;
  left: 11%;
  font-size: 17px;
}

.etichetta-blu:hover, .load-btn:hover{
  background-color: rgb(107, 177, 247);
  cursor: pointer;
  box-shadow: 0px 15px 20px rgba(107, 177, 247, 0.4);
  color: #fff;
  transform: translateY(-7px);
}
.btn-comics{
  text-align: center;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.load-btn{
  border: 1px solid transparent;
  background-color: dodgerblue;
  padding: 10px;
  width: 13%;
  color: white;
  margin-bottom: 20px;
}

.cont-card{
    background-color: rgba($color: #000000, $alpha: 0.9);
}

.container-card{
  width: 80%;
  margin: auto;
  display: flex;
  flex-wrap: wrap;
}
</style>