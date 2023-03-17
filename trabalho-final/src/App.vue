<template>
  
<CorpoSite />
<ContatosSite />
<MissaoSite />
<PeSite/>

</template>

<script>

import CorpoSite from './components/CorpoSite.vue'
import ContatosSite from './components/ContatosSite.vue'
import MissaoSite from './components/MissaoSite.vue'
import PeSite from './components/PeSite.vue'




export default {
  name: 'App',
  components: {
   CorpoSite,
   ContatosSite,
   MissaoSite,
   PeSite
  },
  data() {
    return {
      
    }
  }
}
</script>

<style>
body{
  background-image: url(./assets/universo1.jpg);
}

</style>
