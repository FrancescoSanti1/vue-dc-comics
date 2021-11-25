<template>
    <div id="jumbotron">
        <img src="../assets/img/jumbotron.jpg" alt="">
    </div>
</template>

<script>
export default {
  name: 'Jumbo'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    #jumbotron {
        height: 400px;
        overflow-y: hidden;

        img {
            width: 100%;
        }
    }
</style>