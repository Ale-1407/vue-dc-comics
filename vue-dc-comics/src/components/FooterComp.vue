<template>
    <footer>
        <div class="cont-foot-1">
            <div class="foot-list">
                <div>
                    <ul>
                        <li><h2>DC COMICS</h2></li>
                        <li><span>Characters</span> </li>
                        <li><span>Comics</span> </li>
                        <li><span>Movies</span> </li>
                        <li><span>TV</span> </li>
                        <li><span>Games</span> </li>
                        <li><span>Videos</span> </li>
                        <li><span>News</span> </li>
                    </ul>
                    <ul>
                        <li> <h2>SHOP</h2> </li>
                        <li> <span>Shop DC</span> </li>
                        <li> <span>Shop DC collectibles</span> </li>
                    </ul>
                </div>
                <div>
                    <ul>
                        <li> <span> <h2>DC</h2> </span> </li>
                        <li> <span>Terms Of Use</span> </li>
                        <li> <span>Privacy Policy (New)</span> </li>
                        <li> <span>Ad Choices</span> </li>
                        <li> <span>Advertising</span> </li>
                        <li> <span>Jobs</span> </li>
                        <li> <span>Subscriptions</span> </li>
                        <li> <span>Talent Workshops</span> </li>
                        <li> <span>CPSC Certificates</span> </li>
                        <li> <span>Ratings</span> </li>
                        <li> <span>Shop Help</span> </li>
                        <li> <span>Contact Us</span> </li>
                    </ul>
                </div>
                <div>
                    <ul>
                        <li> <h2>SITES</h2> </li>
                        <li> <span>DC</span> </li>
                        <li> <span>MAD Magazine</span> </li>
                        <li> <span>DC Kids</span> </li>
                        <li> <span>DC Universe</span> </li>
                        <li> <span>DC Power Visa</span> </li>
                    </ul>
                </div>
            </div>
            <div class="foot-img">
                <img src="../assets/img/dc-logo-bg.png" alt="img">
            </div>
        </div>
        <div class="cont-foot-2">
            <div>
                <button class="btn">SIGN-UP NOW!</button>
            </div>
            <div class="icons">
                <ul>
                    <li> <h3>FOLLOW US</h3> </li>
                    <li> <img src="../assets/img/footer-facebook.png" alt=""> </li>
                    <li> <img src="../assets/img/footer-twitter.png" alt=""> </li>
                    <li> <img src="../assets/img/footer-youtube.png" alt=""> </li>
                    <li> <img src="../assets/img/footer-pinterest.png" alt=""> </li>
                    <li> <img src="../assets/img/footer-periscope.png" alt=""> </li>
                </ul>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
  name: 'FooterComp',
}
</script>

<style lang="scss">
.cont-foot-1{
    height: 45vh;
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    display: flex;
    justify-content: space-around;
}

h2{
    color: white;
    padding-bottom: 10px;
}

.foot-list ul{
    padding-top: 1.5rem;
    padding-right: 5rem;
    list-style-type: none;


  li{
    color: grey;
    font-size: 13px;
    font-weight: bold;
    line-height: 20px;
}  
}

.foot-list{
    display: flex;
}

.foot-img img{
    height: -webkit-fill-available;
}

.cont-foot-2{
    height: 11vh;
    background-color: rgba($color: #000000, $alpha: 0.8);
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 9rem;
}

.btn{
    padding: 10px 5px;
    background-color: transparent;
    border: 2px solid dodgerblue;
    color: white;
}

.icons ul{
    list-style-type: none;
    display: flex;
    align-items: center;
    gap: 10px;
}

h3{
    color: dodgerblue;
}
</style>