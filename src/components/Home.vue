<template>
  <v-container id="home-body" fluid>
    <v-layout column align-center>
      <img src="@/assets/mentos.jpg" id="dp" class="mb-3"/>
      <div class="headline mb-1" id="intro-name"><span class="code-color">&lt;</span> Ogundiran Al-Ameen <span class="code-color">&#47&gt;</span></div>
      <div id="nick" class="subheading mb-3">&lt;aka&gt;<span class="aka"> mentos </span>&lt;&#47aka&gt;</div>
      <div id="role" class="subheading mb-3">&lt;skill&gt; <span class="profession">Web and Android Developer</span> &lt;&#47skill&gt;</div>
    </v-layout>
    <v-layout class="mt-3" row wrap>
      <v-flex id="nav-zone" xs12  sm8 offset-sm2 md4 offset-md4>
        <v-layout row wrap>
          <v-flex xs4 text-xs-center>
            <router-link class="link" to="/about" tag="a">About</router-link>
          </v-flex>
          <v-flex xs4 text-xs-center>
            <router-link class="link" to="/projects" tag="a">Projects</router-link>
          </v-flex>
          <v-flex xs4 text-xs-center>
            <router-link class="link" to="/contact" tag="a">Contact</router-link>
          </v-flex>
        </v-layout>
      </v-flex>
    </v-layout>
  </v-container>
</template>


<style scoped>
#home-body {
  cursor: default;
  height: 100%; /* so as to cover full height and background color will be of the entire page */

  background: #136a8a;  /* fallback for old browsers */
  background: -webkit-linear-gradient(to right, #267871, #136a8a);  /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(to right, #267871, #136a8a); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

}
#dp{
  width: 200px;
  margin-top: 5%;
  border-radius: 50%;
  -webkit-border-radius: 50%;
  -moz-border-radius: 50%;
}
#intro-name{
  font-weight: bolder;
  font-family: 'Campton-Bold';
  color: white;
}
.code-color{
  font-family: sans-serif;
  color: #a73737;
  font-weight: bold;
}
#nick{
  color: #a73737; /*#263238*/
}
.aka{
  font-family: 'Campton-Light';
  font-style: italic;
  color: white;
}
#role{
  color: #a73737;
}
.profession{
  color: #ECEFF1;
  font-family: 'Campton-Bold';
  font-style: italic;
}
#nav-zone{
  border: 1px solid #fff;
}
.link{
  color: #263238;
}
.link:hover{
  color: #a73737;
  text-decoration: none;
}
</style>
