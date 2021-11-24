<template>
  <section>
        <div class="container">

            <div class="sites">

                <div>
                    <h4>DC Comics</h4>
                    <ul>
                        <li v-for="comic, i in comics" :key="i">{{comic.text}}</li>
                    </ul>
                </div>

                <div>
                    <h4>DC</h4>
                    <ul>
                        <li v-for="dc, i in dcCom" :key="i">{{dc.text}}</li>
                    </ul>
                </div>

                <div>
                    <h4>Sites</h4>
                    <ul>
                        <li v-for="site, i in sites" :key="i">{{site.text}}</li>
                    </ul>
                </div>

                <div>
                    <h4>Shop</h4>
                    <ul>
                        <li v-for="shop, i in shops" :key="i">{{shop.text}}</li>
                    </ul>
                </div>

                

            </div>

            <div class="logoDC">

                <img src="../assets/img/dc-logo-bg.png" alt="">

            </div>

        </div>
      
  </section>
</template>

<script>
export default {
  name: 'Jumbo',
  data(){
     return {
        comics: [
            {
                text: "Characters",
            },

            {
                text: "Comics",
            },

            {
                text: "Movies",
            },

            {
                text: "TV",
            },

            {
                text: "Games",
            },

            {
                text: "Videos",
            },

            {
                text: "News",
            }
        ],

        dcCom: [
            {
                text: "Terms of Use",
            },

            {
                text: "Privacy Policy (New)",
            },

            {
                text: "Ad Choices",
            },

            {
                text: "Advertising",
            },

            {
                text: "Jobs",
            },

            {
                text: "Subscriptions",
            },

            {
                text: "Talent Workshops",
            },

            {
                text: "CPSC Certificates",
            },

            {
                text: "Ratings",
            },

            {
                text: "Shop Help",
            },

            {
                text: "Contact Us",
            }

        ],
        sites: [
            {
                text: "DC",
            },

            {
                text: "MAD Magazines",
            },

            {
                text: "DC Kids",
            },

            {
                text: "DC Universe",
            },

            {
                text: "DC Power Visa",
            }
        ],

        shops: [
            {
                text: "Shop DC",
            },

            {
                text: "Shop DC Collectibles",
            }
        ]
     }
    }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    section {
        height: 400px;
        background-image: url("../assets/img/footer-bg.jpg");
        background-repeat: no-repeat;
        background-size: cover;

        .container {
            width: 80%;
            margin: auto;

            .logoDC img {
                height: 400px;
                width: 600px;
                float: right;
                object-fit: none;
                
            }

            .sites{
                float: left;
                margin-top: 20px;
                display: flex;
                justify-content: space-between;
                flex-wrap: wrap;

                div {
                    width: calc(100% / 3 - 10px);
                    margin-right: 10px;
                }

                h4 {
                    color: white;
                    text-transform: uppercase;
                }

                li {
                list-style-type: none;
                font-size: 10px;
                color: #808A89;
                margin-top: 5px;
            }
            }

            
        }
    }
    
</style>
