<template>
  
    <div id="jumbotron">
        <!-- Sezione delle liste -->
        <section id="list">

            <!-- Liste di sinistra -->
            <section id="list_left">

                <!-- Lista di sopra -->
                <div id="list_sopra">
                    <h1>DC COMICS</h1>
                    <ul>
                        <li v-for="link, i in links_1" :key="i">
                            <a href="">{{link.text}}</a>
                        </li>
                    </ul>
                </div>

                <!-- Lista di sotto -->
                <div id="list_sotto">
                    <h1>SHOP</h1>
                    <ul>
                        <li v-for="link, i in links_2" :key="i">
                            <a href="">{{link.text}}</a>
                        </li>
                    </ul>
                </div>
            </section>

            <!-- Lista centrale -->
            <section id="list_center">
                <h1>DC</h1>
                <ul>
                    <li v-for="link, i in links_3" :key="i">
                        <a href="">{{link.text}}</a>
                    </li>
                </ul>
            </section>

            <!-- Lista di destra -->
            <section id="list_right">
                <h1>SITES</h1>
                <ul>
                    <li v-for="link, i in links_4" :key="i">
                        <a href="">{{link.text}}</a>
                    </li>
                </ul>
            </section>
        </section>

        <!-- Sezione del secondo sfondo -->
        <section id="img_sfondo">
        </section>
      
    </div>




</template>

<script>
export default {
  name: "Jumbo",
  data() {
      return {

        //   links per la lista di sopra
          links_1 : [
              
              {
                  'text': "Characters",
                  'url': "",
              },

               {
                  'text': "Comics",
                  'url': "",
              },

               {
                  'text': "Movies",
                  'url': "",
              },

               {
                  'text': "TV",
                  'url': "",
              },

               {
                  'text': "Games",
                  'url': "",
              },

               {
                  'text': "Video",
                  'url': "",
              },

               {
                  'text': "News",
                  'url': "",
              }
          ],

        // links per la lista di sotto 
          links_2 : [

              {
                  'text': "Shop DC",
                  'url': "",
              },

               {
                  'text': "Shop DC Collectibles",
                  'url': "",
              }
          ],

        // link le per la lista centrali
            links_3 : [

                {
                  'text': "Terms Of Use",
                  'url': "",
                },

               {
                  'text': "Privacy policy (New)",
                  'url': "",
                },

               {
                  'text': "Ad Choices",
                  'url': "",
                },

               {
                  'text': "Advertising",
                  'url': "",
                },

               {
                  'text': "Jobs",
                  'url': "",
                },

               {
                  'text': "Subscriptions",
                  'url': "",
                },

               {
                  'text': "Talent Workshops",
                  'url': "",
                },

                {
                  'text': "CPSC Certificates",
                  'url': "",
                },

               {
                  'text': "Ratings",
                  'url': "",
                },

               {
                  'text': "Shop Help",
                  'url': "",
                },

               {
                  'text': "Contact Us",
                  'url': "",
                }
            ],

        // link per la lista di destra
            links_4 : [

                {
                  'text': "DC",
                  'url': "",
                },

                {
                  'text': "MAD Magazine",
                  'url': "",
                },

                {
                  'text': "DC Kids",
                  'url': "",
                },

                {
                  'text': "DC Universe",
                  'url': "",
                },

                {
                  'text': "DC Power Visa",
                  'url': "",
                }
            ]
        }
    }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

    #jumbotron {
        background-image: url("../../public/assets/img/footer-bg.jpg");
        width: 100%;
        height: 400px;

    
        #list {
            float: left;
            width: 50%;
            height: 100%;
            padding: 20px 0 0 14% ;

            #list_left, #list_center, #list_right {

                float: left;
                padding: 0 2.5%;
            }            

            h1 {
                color: white;
                padding-bottom: 15px;
                padding: 10% 0 3% 0;
            }

            ul {
                list-style-type: none;

                li {
                    padding: 5px 0;

                    a {

                        text-decoration: none;
                        color: grey;

                        &:hover {

                            color: lightgrey;
                        }
                    }

                }
            }

            
        }
        
        #img_sfondo {
            float: left;
            width: 40%;
            height: 100%;
            margin: 0;
            padding-right: 14%;
            background-image: url("../../public/assets/img/dc-logo-bg.png");
            background-size: cover;
        }
    }
    
</style>