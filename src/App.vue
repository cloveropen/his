<template>
  <v-app>
    <v-app-bar app style="background-color:darkgray" height="60">
      <span><v-img :src="require('./assets/logo.svg')"  contain height="70"  width="60"  position="left top"></v-img>
      </span>
      <v-toolbar-title class="headline text-uppercase" >
      
        <span ><a href="http://www.cloveropen.com/" style="color:antiquewhite">苜蓿草科技</a></span>
        <!-- <span class="font-weight-light">&nbsp;&nbsp;www.cloveropen.com</span>  -->
      </v-toolbar-title>
      <v-spacer></v-spacer>

        <span class="mr-2">v0.0.1</span>
  

    </v-app-bar>

    <v-content style="background-color:darkgray" >
     
      <HelloWorld/>
     
    </v-content>
    
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';
export default {
  name: 'App',
  components: {
    HelloWorld,
  },
  data: () => ({
    //
  }),
};
</script>

<style  lang='scss'>
.mr-2{
  color:antiquewhite;
}
</style>
