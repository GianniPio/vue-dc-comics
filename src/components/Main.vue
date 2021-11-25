<template>
  <main>
      <!-- Stampa elementi array -->
      <ul>
          <li v-for= "link, i in links" :key="i">
              <img :src="link.img" alt=""/>
              <a href="">{{link.text}}</a>
          </li>
      </ul>
  </main>
</template>

<script>
export default {
  name: "Main",
  data() {
      return {
          links : [
              {
                  'text': "DIGITAL COMICS",
                  'img': "assets/img/buy-comics-digital-comics.png"
              },

               {
                  'text': "DC MERCHANDISE",
                  'img': "assets/img/buy-comics-merchandise.png"
              },

               {
                  'text': "SUBSCRIPTION",
                  'img': "assets/img/buy-comics-subscriptions.png"
              },

               {
                  'text': "COMIC SHOP LOCATOR",
                  'img': "assets/img/buy-comics-shop-locator.png"
              },

               {
                  'text': "DC POWER VISA",
                  'img': "assets/img/buy-dc-power-visa.svg"
              }
          ]
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

    main {

        background-color: #0282f9;
        width: 100%;
        height: 140px;
        padding: 1% 14%;
        
        ul {
            list-style-type: none;
            line-height: 600%;
            display: flex;
            justify-content: space-between;

            img {
                width: 25%;
                display: inline-block;
                vertical-align: middle;
            }

            li {
                
                margin: 0 20px;
                width: calc(100% / 5);

                a {
                    text-decoration: none;
                    color: white;
                    font-size: 10px;
                    display: inline;
                    }

            }
            
            
            
        }
    }

</style>
