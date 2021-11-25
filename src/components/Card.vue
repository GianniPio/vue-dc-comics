// Figlio di ContentBlack, serve per la stampa dell'array

<template>

    <!-- Elemento dell'array -->
  <div class="card">
      <section class="copertina">
          <img :src="details.thumb" :alt="details.series">
          </section>
      <p>{{details.series}}</p>
      <span>{{details.price}}</span>
  </div>
  
</template>

<script>
export default {
  name: "Card",
  props: {
      details: Object,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

    .card {
        width: calc(100% / 6);
        height: 100%;
        display: inline-block;
        padding: 2% 0;

        p,span {
            font-size: 10px;
        }

        .copertina {
            height: auto;
            width: 150px;

            img {
                object-fit: contain;
                width: 100%;
                height: 100%;
            }
        }
        
    }

    
</style>