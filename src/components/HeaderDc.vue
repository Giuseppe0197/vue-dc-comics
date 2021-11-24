<template>
  <header>
      <img src="../assets/img/dc-logo.png" alt="">

      <ul>
          <li v-for="link, i in links" :key="i" :class="link.visuability === true ? 'active' : ''">{{link.text}}</li>
      </ul>
  </header>
</template>

<script>
export default {
  name: 'HeaderDc',

 data(){
     return {
         links: [
             {
                 text: "Characters",
                 visuability: false
             },

             {
                 text: "Comics",
                 visuability: true
             },

             {
                 text: "Movies",
                 visuability: false
             },

             {
                 text: "TV",
                 visuability: false
             },

             {
                 text: "Games",
                 visuability: false
             },

             {
                 text: "Collectibles",
                 visuability: false
             },

             {
                 text: "Videos",
                 visuability: false
             },

             {
                 text: "Fans",
                 visuability: false
             },

             {
                 text: "News",
                 visuability: false
             },

             {
                 text: "Shop",
                 visuability: false
             }
         ]
     }
 }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
    width: 80%;
    margin: auto;
    height: 145px;

    img {
        float: left;
        margin-top: 30px;
        width: 80px;
    }

    ul {
        float: right;

        li {
            display: inline-block;
            margin: 0 10px;
            line-height: 140px;
            text-transform: uppercase;
            font-size: 12px;
            font-weight: bold;

            &:hover {
                color: blue;
                cursor: pointer;
            }

            &.active{
                color: blue;
                border-bottom: 5px solid blue;
            }
        }
    }

    
}
    
</style>
