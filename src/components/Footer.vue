<template>
  <footer>
      <!-- Sezione per il bottone -->
      <section id="btn">
          <button>SIGN-UP NOW!</button>
      </section>

    <!-- Sezione social -->
      <section id="social">
          <h3>FOLLOW US</h3>
          <ul>
              <li v-for="link, i in links" :key="i">
                  <img :src="link.img" alt="">
                  <a href="link.url"></a>
              </li>
          </ul>

      </section>

  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
      return {
          links : [
                {
                  'url': "",
                  'img': ""
                },

                {
                  'url': "",
                  'img': "assets/img/footer-facebook.png"
                },

                {
                  'url': "",
                  'img': "assets/img/footer-twitter.png"
                },

                {
                  'url': "",
                  'img': "assets/img/footer-youtube.png"
                },

                {
                  'url': "",
                  'img': "assets/img/footer-pinterest.png"
                },

                {
                  'url': "",
                  'img': "assets/img/footer-periscope.png"
                }
          ]
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

  footer {
      background-color: #303030;
      height: 115px;
      padding: 0 14%;
      vertical-align: middle;

      #btn {
          float: left;
          width: 40%;
          height: 100%;
          display: flex;
          justify-content: center;
          padding: 3% 1%;

          button {
              border: 3px solid #0282f9;
              padding: 1% 4%;
              background-color: #303030;
              color: white;
              font-weight: bold;
              cursor: pointer;

              &:hover {
                  background-color: grey;
              }
              
          }
      }

      #social {
          float: right;
          width: 40%;
          height: 100%;
          display: flex;
          flex-direction: row;
          padding: 4% 0;
          align-items: center;

          h3 {
              color: #0282f9;
              padding-right: 5%;
          }

          ul {
              display: flex;
              list-style-type: none;

              li {
                  vertical-align: middle;
                  padding:  0 2%;
                  
                  img {
                      cursor: pointer;

                      &:hover {
                          filter: brightness(1%);
                      }
                  }
              }
          }

      }
  }

</style>
