<template>
  
      <div class="thumbsComics">
            <img :src="details.thumb" alt="">
            <p>{{details.series}}</p>
            <p class="typeCom">{{details.type}}</p>
            <p class="priceCom">{{details.price}}</p>

        </div>
  
</template>

<script>
export default {
  name: 'thumbComp',
  props: {
      details: Object
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .thumbsComics {
        width: calc(100% / 6);
        

        img {
            width: 100%;
            object-fit: none;
            object-position: top;
            height: 70%;
        }

        p {
            color: white;

            &.typeCom, &.priceCom {
                margin-top: 5px;
            }

        }
    }
    
</style>
