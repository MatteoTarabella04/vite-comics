<script>

import appHeader from './components/_header.vue';
import appMain from './components/_main.vue';
import appFooter from './components/_footer.vue';

export default {
  components: {
    appHeader,
    appMain,
    appFooter,
  }

}
</script>

<template>
  <appHeader />

  <appMain />

  <appFooter />
</template>


<style lang="scss" scoped></style>