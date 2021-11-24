<template>
  <section>
      <div>
          <ul>
              <li v-for="merch, i in merches" :key="i"><img :src="merch.imgMerch">{{merch.text}}</li>
          </ul>
      </div>
  </section>
</template>

<script>
export default {
  name: 'Merchandise',

  data(){
     return {
        merches: [
            {
                imgMerch: "../assets/img/buy-comics-digital-comics.png",
                text: "Digital Comics",
                visuability: false
            },

            {
                imgMerch: "../assets/img/buy-comics-merchandise.png",
                text: "DC Merchandise",
                visuability: true
            },

            {
                imgMerch: "../assets/img/buy-comics-shop-locator.png",
                text: "Subscription",
                visuability: false
            },

            {
                imgMerch: "../assets/img/buy-comics-subscriptions.png",
                text: "Comic Shop Locator",
                visuability: false
            },

            {
                imgMerch: "../assets/img/buy-dc-power-visa.svg",
                text: "DC Power Visa",
                visuability: false
            }
        ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section{
    background-color: #0282F9;
    height: 140px;

    div {
        width: 75%;
        margin: auto;

        img {
            color: white;
            width: 50px;
        }

        li {
            display: inline-block;
            margin: 30px;
        }

        
    }
}
</style>