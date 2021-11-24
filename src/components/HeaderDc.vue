<template>
  <header>
      <section>
          <img src="../assets/img/dc-logo.png" alt="">

        <ul>
            <li v-for="link, i in links" :key="i" :class="link.visuability === true ? 'active' : ''">{{link.text}}</li>
        </ul>
      </section>
      
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
    height: 145px;

    section {
        width: 80%;
        margin: auto;

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
                margin-top: 60px;
                text-transform: uppercase;
                font-size: 12px;
                font-weight: bold;

                &:hover {
                    color: blue;
                    cursor: pointer;
                }

                &.active{
                    color: blue;
                    padding-bottom: 66px;
                    border-bottom: 5px solid blue;
                }
            }
        }
    }

    

    
}
    
</style>
