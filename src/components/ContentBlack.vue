<template>

  <div id="section_black">
    <!-- Immagine di Jumbotron -->
    <section id="img_jumbo">
    </section>

    <div id="box">
      <h3>CURRENT SERIES</h3>
    </div>

    <!-- Sezione della stampa degli elementi dell'array, tramite props -->
    <div class="card_comics">      
      <Card v-for="comic, i in comics" :key="i" :details="comic"/>
  </div>

  <div id="more">
    <h5>LOAD MORE</h5>
  </div>
</div>
  
</template>

<script>
import Card from "@/components/Card.vue";  //ho messo @ perché altrimenti non funziona, import del figlio, da aggiugere poi in components

export default {
 name: "ContentBlack",
 components: {
   Card,
 },
 data() {
      return {
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

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

  #section_black {

    position: relative;

    #box {
      width: auto;
      padding: 10px;
      background-color: #0282f9;
      position: absolute;
      top: 24%;
      left: 15%;
      
       h3 {
         color: white;

       }
    }

    #img_jumbo {
      background-image: url("../../public/assets/img/jumbotron.jpg");
      width: 100%;
      height: 240px;
      background-size: cover;
      }

    .card_comics {
      background-color: #1c1c1c;
      padding: 15px 14% 50px;
      color: white;
    }

    #more {
      position: absolute;
      background-color: #0282f9;
      bottom: 1px;
      left: 50%;
      padding: 7px 50px;
      transform: translate(-50%, -50%);

        h5 {
          color: white;
          width: auto;

        }
    }

  }
    
 

  

    
    
</style>
