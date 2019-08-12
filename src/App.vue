<template>
  <v-app>
    <v-app-bar app>
      <v-toolbar-title class="headline text-uppercase">
        <span><a href="http://www.cloveropen.com/">苜蓿草科技</a></span>
        <!-- <span class="font-weight-light">&nbsp;&nbsp;www.cloveropen.com</span>  -->
      </v-toolbar-title>
      <v-spacer></v-spacer>

        <span class="mr-2">v0.0.1</span>
      </v-btn>
    </v-app-bar>

    <v-content>
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
