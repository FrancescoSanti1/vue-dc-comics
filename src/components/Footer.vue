<template>
    <footer>
        <div id="footer-top">
            <div class="container">
                <nav v-for="(list, i) in footerLists" :key="i">
                    <h3>{{list.listName}}</h3>
                    <ul>
                        <li v-for="(item, j) in list.listItems" :key="j">
                            <a :href="item.path">{{item.text}}</a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
        <div id="footer-bottom">
            <div class="container">
                <div class="btn">sign-up now!</div>
                <div id="social">
                    <div class="text">follow us</div>
                    <div class="icons">
                        <img src="../assets/img/footer-facebook.png" alt="">
                        <img src="../assets/img/footer-periscope.png" alt="">
                        <img src="../assets/img/footer-pinterest.png" alt="">
                        <img src="../assets/img/footer-twitter.png" alt="">
                        <img src="../assets/img/footer-youtube.png" alt="">
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
  name: 'Footer',
  data() {
      return {
          footerLists: [
              {
                  listName: "dc comics",
                  listItems: [
                      {
                          text: "Characters",
                          path: "#"
                      },
                      {
                          text: "Comics",
                          path: "#"
                      },
                      {
                          text: "Movies",
                          path: "#"
                      },
                      {
                          text: "TV",
                          path: "#"
                      },
                      {
                          text: "Games",
                          path: "#"
                      },
                      {
                          text: "Videos",
                          path: "#"
                      },
                      {
                          text: "News",
                          path: "#"
                      }
                  ]
              },
              {
                  listName: "shop",
                  listItems: [
                      {
                          text: "Shop DC",
                          path: "#"
                      },
                      {
                          text: "Shop DC Collectibles",
                          path: "#"
                      }
                  ]
              },
              {
                  listName: "dc",
                  listItems: [
                      {
                          text: "Terms of use",
                          path: "#"
                      },
                      {
                          text: "Privacy policy",
                          path: "#"
                      },
                      {
                          text: "Advertising",
                          path: "#"
                      },
                      {
                          text: "Subscription",
                          path: "#"
                      },
                      {
                          text: "Contact Us",
                          path: "#"
                      }
                  ]
              },
              {
                  listName: "sites",
                  listItems: [
                      {
                          text: "DC",
                          path: "#"
                      },
                      {
                          text: "MAD Magazine",
                          path: "#"
                      },
                      {
                          text: "DC Universe",
                          path: "#"
                      },
                      {
                          text: "DC Power Visa",
                          path: "#"
                      }
                  ]
              }
          ]
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    footer {

        #footer-top {

            background-image: url("../assets/img/footer-bg.jpg");
        
            .container {
                padding: 50px 0;
                background-image: url("../assets/img/dc-logo-bg.png");
                background-repeat: no-repeat;
                background-position: right center;
                display: flex;
                flex-direction: column;
                flex-wrap: wrap;
                align-content: flex-start;
                // debug
                height: 350px;

                nav {
                    margin: 0 10px 20px 0;

                    h3 {
                        text-transform: uppercase;
                        color: white;
                    }

                    ul {
                        list-style-type: none;

                        a {
                            font-size: 12px;
                            color: grey;
                            text-decoration: none;
                        }
                    }
                }
            }
        }

        #footer-bottom {
            background-color: #303030;

            .container {
                height: 150px;
                display: flex;
                justify-content: space-between;
                align-items: center;

                .btn {
                    color: white;
                    text-transform: uppercase;
                    padding: 10px;
                    border: 2px solid #0282f9;
                }

                #social {

                    display: flex;
                    align-items: center;

                    .text {
                        color: #0282f9;
                        text-transform: uppercase;
                        font-weight: bold;
                        margin-right: 10px;
                    }

                    .icons {

                        img {
                            height: 30px;
                            margin: 0 10px;
                        }          
                    }
                }


            }
        }
        
    }
</style>