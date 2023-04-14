<script>

import sectionIconBar from './_iconBar.vue';

export default {

   name: 'appMain',

   components: {
      sectionIconBar,
   },

   data() {
      return {

      }
   }

}
</script>

<template>
   <main class="bg-dark">
      <section id="main_sec">
         <div class="container">
            <h3 class="m-0 py-5 text-white">-- Content Goes Here --</h3>
         </div>
         <!-- /.container -->
      </section>
      <!-- /#main_sec -->

      <sectionIconBar />
      <!-- /sectionIconBar -->

   </main>
</template>



<style lang="scss" scoped></style>