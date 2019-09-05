<template>
  <v-app>
    <v-content>
      <Jumbotron/>
      <Cards/>
      <Cobertura/>
      <HelloWorld/>
      <BottomNav/>
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import Jumbotron from './components/Jumbotron'
import Cards from './components/Cards'
import Cobertura from './components/Cobertura'
import BottomNav from './components/BottomNav'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Jumbotron,
    Cards,
    Cobertura,
    BottomNav,
  },
  data: () => ({
    //
  }),
};
</script>
