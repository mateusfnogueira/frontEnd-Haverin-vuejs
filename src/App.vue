<template>
  <v-app>
    <Header />
    
      <transition name="slide" mode="out-in">
        <router-view></router-view>
      </transition>
    
    <Footer />
  </v-app>
</template>

<script>
import Header from "./components/Header";
import Footer from "./components/Footer"

export default {
  components: {
    Header,
    Footer
  },
};
</script>

<style lang="scss">
.menu-header-mobile {
  a {
    text-decoration: none;
    color:coral !important;
  }
}
@keyframes slide-in {
  from {
    transform: translateY(-30px);
    opacity: 0;
  }
  to {
    transform: translateY(0px);
    opacity: 1;
  }
}

@keyframes slide-out {
  from {
    transform: translateY(0px);
    opacity: 1;
  }
  to {
    transform: translateY(-30px);
    opacity: 0;
  }
}

.slide-enter-active {
  animation: slide-in 0.3s ease;
}

.slide-leave-active {
  animation: slide-out 0.3s ease;
}
</style>
