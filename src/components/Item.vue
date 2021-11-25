<template>
    <div class="item">
        <div class="img-container">
            <img :src="img" :alt="text">
        </div>
        <h4>{{text}}</h4>
    </div>
</template>

<script>
export default {
  name: 'Item',
  props: {
      img: String,
      text: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .item {
        width: 15%;

        .img-container {
            padding-top: 100%;
            position: relative;
            overflow-y: hidden;

            img {
                position: absolute;
                top: 0;
                left: 0;
                width: 100%;
            }
        }

        h4 {
            text-transform: uppercase;
            font-weight: normal;
            font-size: 14px;
            margin: 10px 0 20px;
        }
    }
    
</style>