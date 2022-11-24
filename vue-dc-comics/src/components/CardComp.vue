<template>
    <div class="card">
        <div>
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
</style>