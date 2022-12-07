<template >
  <div>
    <header>
      <v-header ></v-header>
    </header>
    <main>
      <section>
        <v-body></v-body>
      </section>
    </main>
    <footer>
<v-footer></v-footer>
    </footer>
  </div>
</template>
<script>
import HeaderVue from '@/assets//Component/Header.vue';
import BodyVue from './assets/Component/Body.vue';
import FooterVue from './assets/Component/Footer.vue';
export default {
  
  components:{
    'v-header':HeaderVue,
    'v-body':BodyVue,
    'v-footer':FooterVue
  }
}
</script>
<style >
body{
  background-color: hsl(180, 23%, 21%);
}
</style>