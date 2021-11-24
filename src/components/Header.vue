<template>
  <header>
    <img src="assets\img\dc-logo.png" alt="ciao">
    <div id="listmenu">
        <ul>
            <li v-for= "link, i in links" :key="i">
                <a href="link.url">{{link.text}}</a>
            </li>
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
        height: 20%;
        width: 100%;
        display: flex;
        justify-content: space-between;
        padding: 0 14%;
        font-size: 12px;

        img {
            padding: 20px
        }
    
        #listmenu ul {
            display: flex;
            list-style-type: none;
            line-height: 1000%;

            li {
                margin: 10px;
                font-weight: bold;
                

                a {
                    color: black;
                    text-decoration: none;

                    &:hover {
                        padding-bottom: 61px;
                        color: #0282f9;
                        border-bottom: 5px solid #0282f9;
                    }
                }

                &.active {
                    color: #0282f9;
                }
            }
        }
        
    }
</style>
