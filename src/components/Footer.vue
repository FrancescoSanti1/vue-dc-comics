<template>
    <footer>
        <div class="container">
            <nav>
                <h3>dc comics</h3>
                <ul>
                    <li>
                        <a href="">Voce 1</a>
                    </li>
                    <li>
                        <a href="">Voce 1</a>
                    </li>
                    <li>
                        <a href="">Voce 1</a>
                    </li>
                </ul>
            </nav>
            <nav>
                <h3>dc comics</h3>
                <ul>
                    <li>
                        <a href="">Voce 1</a>
                    </li>
                    <li>
                        <a href="">Voce 1</a>
                    </li>
                    <li>
                        <a href="">Voce 1</a>
                    </li>
                </ul>
            </nav>
            <nav>
                <h3>dc comics</h3>
                <ul>
                    <li>
                        <a href="">Voce 1</a>
                    </li>
                    <li>
                        <a href="">Voce 1</a>
                    </li>
                    <li>
                        <a href="">Voce 1</a>
                    </li>
                </ul>
            </nav>        
        </div>
    </footer>
</template>

<script>
export default {
  name: 'Footer',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    footer {
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
            height: 300px;

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
</style>