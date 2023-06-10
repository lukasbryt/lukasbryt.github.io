<script>
import { RouterLink, RouterView } from 'vue-router'
import NameBar from './components/NameBar.vue'
import Footer from './components/Footer.vue';
export default {
  components: { NameBar, RouterLink, Footer }
}
</script>
<template>
  <main>
    <div class="container">
      <NameBar />
    </div>
    <router-view v-slot="{ Component }">
      <transition name="page-opacity" mode="out-in">
        <component :is="Component" :key="$route.path"></component>
      </transition>
    </router-view>
  </main>
  <Footer /> 
</template>
<style scope>
.page-opacity-enter-active,
.page-opacity-leave-active {
  transition: opacity 0.6s, transform 0.6s;
}

.page-opacity-enter-from,
.page-opacity-leave-to {
  opacity: 0;
}
</style>
