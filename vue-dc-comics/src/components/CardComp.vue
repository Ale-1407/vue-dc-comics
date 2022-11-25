<template>
    <div class="card">
        <div class="card-img">
           <img :src="dettagliComics.thumb" alt=""> 
        </div>
        <div>
            <h4>{{ dettagliComics.series }}</h4>
        </div>
    </div>
</template>

<script>
export default {
  name: 'CardComp',
  props: {
    dettagliComics: Object
  }
}
</script>

<style lang="scss">

.card{
    width: calc(100% / 6);
    padding: 15px;
}

h4{
    padding-top: 10px;
}

.card-img img{
    width: 100%;
    aspect-ratio: 1/1;
    object-fit:cover;
    object-position: top;
}

.card-img img:hover{
    box-shadow: 0px 15px 20px rgba(107, 177, 247, 0.4);
    cursor: pointer;
}
</style>