<template>
    <div id="app">
        <div class="js-Landing">
            <img src="~assets/vg.png">
            <h1>{{ msg }}</h1>
            <a class="button--default" :href="zorkoVgcodeUrl">Try It!</a>

            <h2>Essential Link</h2>
            <ul>
                <li><a href="http://example.com" target="_blank">Twitter</a></li>
                <li><a href="http://example.com" target="_blank">Discuss</a></li>
                <li><a href="http://example.com" target="_blank">Slack</a></li>
                <li><a href="http://example.com" target="_blank">Issues</a></li>
            </ul>
        </div>
    </div>
</template>

<script>
  export default {
    name: 'landing',

    data () {
      return {
        msg: 'Welcome to Vega Code'
      }
    },

    asyncData ({ env }) {
      return {
        zorkoVgcodeUrl: env.zorkoVgcodeUrl
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }

    .button--default {
        font-size: 1.2em;
        padding: 0.75em 2em;
        border-radius: 2em;
        display: inline-block;
        color: #fff;
        background-color: #4fc08d;
        transition: all 0.15s ease;
        box-sizing: border-box;
        border: 1px solid #4fc08d;
    }

    h1, h2 {
        font-weight: normal;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        display: inline-block;
        margin: 0 10px;
    }

    li a {
        color: #42b983;
    }

</style>
