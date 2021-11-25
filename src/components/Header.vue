<template>
    <header>
        <div class="container">
            <div id="logo">
                <img src="../assets/img/dc-logo.png" alt="logo dc comics">
            </div>
            <nav>
                <ul>
                    <li v-for="object, i in navList" :key="i">
                        <a :href="object.path">{{object.text}}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
      return {
          navList: [
              {
                  text: "characters",
                  path: "#"
              },
              {
                  text: "comics",
                  path: "#"
              },
              {
                  text: "movies",
                  path: "#"
              },
              {
                  text: "tv",
                  path: "#"
              },
              {
                  text: "games",
                  path: "#"
              },
              {
                  text: "collectibles",
                  path: "#"
              },
              {
                  text: "videos",
                  path: "#"
              },
              {
                  text: "fans",
                  path: "#"
              },
              {
                  text: "news",
                  path: "#"
              },
              {
                  text: "shop",
                  path: "#"
              }
          ]
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    header {

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 150px;
        }

        li {
            display: inline-block;
            text-transform: uppercase;
            margin: 0 10px;

            a {
                color: black;
                text-decoration: none;
            }
        }
    }
</style>