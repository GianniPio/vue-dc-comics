<template>
  <header>
    <img src="..\assets\img\dc-logo.png" alt="">
    <div id="listmenu">
        <ul>
            <li v-for= "link, i in links" :key="i">{{link.text}}</li>
        </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
      return {
          links : [
              {
                  'text': "CHARACTERS",
                  'url': "",
                  'clicked': false
              },

               {
                  'text': "COMICS",
                  'url': "",
                  'clicked': true
              },

               {
                  'text': "MOVIES",
                  'url': "",
                  'clicked': false
              },

               {
                  'text': "TV",
                  'url': "",
                  'clicked': false
              },

               {
                  'text': "GAMES",
                  'url': "",
                  'clicked': false
              },

               {
                  'text': "COLLECTIBLES",
                  'url': "",
                  'clicked': false
              },

               {
                  'text': "VIDEOS",
                  'url': "",
                  'clicked': false
              },

               {
                  'text': "FANS",
                  'url': "",
                  'clicked': false
              },

               {
                  'text': "NEWS",
                  'url': "",
                  'clicked': false
              },

               {
                  'text': "SHOP",
                  'url': "",
                  'clicked': false
              }
          ]
      }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    header {
        border: 1px solid black;
        height: 20%;
        display: flex;
        justify-content: space-around;

        img {
            padding: 20px
        }
    
        #listmenu ul {
            display: flex;
            list-style-type: none;
            line-height: 700%;

            li {
                margin: 10px;
                font-weight: bold;

                &:hover {
                    color: #0282f9;
                }

                &.active {
                    color: #0282f9;
                }
            }
        }
        
    }
</style>
