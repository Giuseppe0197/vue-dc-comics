<template>
  <section>
        <div class="container">

            <div class="sites">

                <div>
                    <h4>DC Comics</h4>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                </div>

                <div>
                    <h4>DC</h4>
                    <ul>
                        <li>Terms Of Use</li>
                        <li>Privacy Policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>

                <div>
                    <h4>Sites</h4>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>

                <div>
                    <h4>Shop</h4>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>

                

            </div>

            <div class="logoDC">

                <img src="assets/img/dc-logo-bg.png" alt="">

            </div>

        </div>
      
  </section>
</template>

<script>
export default {
  name: 'Jumbo',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    section {
        height: 400px;
        background-image: url("../../public/assets/img/footer-bg.jpg");
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
