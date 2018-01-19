<template>
  <v-app>
    <v-content>
      <router-view/>
    </v-content>
    <v-footer id="footer" :fixed="fixed" app>
      <div id="footer-text" class="text-xl-center"><p>&copy; {{year}}. Built with <span class="heart">&#10085;</span> by <a target="_blank" href="http://twitter.com/piomentos">mentOS</a> <span class="knight">&#9822</span></p></div>
    </v-footer>
  </v-app>
</template>

<script>
var yr = new Date().getFullYear()
export default {
  data () {
    return {
      fixed: false,
      year: yr
    }
  },
  name: 'App'
}
</script>
<style scoped>
#footer{
  background-color: #263238;
  color: white;
}
#footer-text{
    margin: 0 auto;
    margin-top: 6px;
}
.heart{
  color: #FF7043;
  /* other html heart codes - &#9829; &#10084 &#10085*/
}
.knight{
  color: #00BCD4;
}
@font-face {
  font-family: 'Campton-Light';
  src: url('/static/fonts/Campton-Light.otf') format("opentype");
}
@font-face {
  font-family: 'Campton-Bold';
  src: url('/static/fonts/Campton-Bold.otf') format("opentype");
}
</style>
