<template>
  <div id="header">
    <img src="..\assets\img\dc-logo.png" alt="">
    <div id="listmenu">
        <ul>
            <li>home</li>
            <li>asd</li>
            <li>asd</li>
            <li>CIao</li>
            <li>CIao</li>
            <li>CIao</li>
            <li>CIao</li>
            <li>CIao</li>
            <li>CIao</li>
            <li>CIao</li>
        </ul>
    </div>
    
  </div>
</template>

<script>
export default {
  name: "Header",
  
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    #header {
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
            }
        }
        
    }

    li:hover {
        color: #0282f9;
    }

    li.active {
        color: #0282f9;
    }
</style>
