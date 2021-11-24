<template>
  <section>

      <div class="containerFooter">
          <button>Sign Up Now!</button>

          

          <!-- <ul>
              <li><img src="../assets/img/footer-facebook.png" alt=""></li>
              <li><img src="../assets/img/footer-twitter.png" alt=""></li>
              <li><img src="../assets/img/footer-youtube.png" alt=""></li>
              <li><img src="../assets/img/footer-pinterest.png" alt=""></li>
              <li><img src="../assets/img/footer-periscope.png" alt=""></li>
          </ul> -->

          <ul>
              <li v-for="social, i in footerSocial" :key="i"><img :src="require(`../assets/img/${social.imgFooter}`)"/></li>
          </ul>

          <span>Follow Us</span>
      </div>

      

  </section>
</template>

<script>
export default {
  name: 'Footer',

  data(){
     return {
        footerSocial: [
            {
                imgFooter: "footer-facebook.png",
                visuability: false
            },

            {
                imgFooter: "footer-twitter.png",
                visuability: false
            },

            {
                imgFooter: "footer-youtube.png",
                visuability: false
            },

            {
                imgFooter: "footer-pinterest.png",
                visuability: false
            },

            {
                imgFooter: "footer-periscope.png",
                visuability: false
            }
        ]
    }
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    section {
        height: 100px;
        background-color: #303030;

        .containerFooter {
            width: 80%;
            margin: auto;
        }

        button {
            font-size: 30px;
            border: 2px solid #008CFF;
            background-color: transparent;
            color: white;
            padding: 10px;
            margin-top: 20px;
        }

        span {
            float: right;
            margin-right: 20px;
            line-height: 100px;
            color: #008CFF;
            text-transform: uppercase;
            font-weight: bold;
        }

        ul {
            float: right;

            li {
                display: inline-block;
                margin-right: 20px;
                line-height: 120px;
            }
        }
    }
</style>