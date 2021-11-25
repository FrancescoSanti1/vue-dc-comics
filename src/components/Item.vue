<template>
    <div class="item">
        <img :src="img" :alt="text">
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

        h4 {
            text-transform: uppercase;
            font-weight: normal;
            margin: 10px 0 20px;
        }
    }
    
</style>