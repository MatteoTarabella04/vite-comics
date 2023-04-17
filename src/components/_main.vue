<script>

import sectionIconBar from './_iconBar.vue';
import jumbotron from './_jumbotron.vue';
import comics from './_comics.vue';

export default {

   name: 'appMain',

   components: {
      sectionIconBar,
      jumbotron,
      comics,
   },

   data() {
      return {

      }
   }

}
</script>

<template>
   <main id="app_main" class="bg-dark">

      <jumbotron />
      <section id="main_sec">
         <div class="container">
            <div class="tag bg-primary text-white text-uppercase text-center">
               <h4 class="m-0"><strong>current series</strong></h4>
            </div>
         </div>
         <comics />
      </section>
      <!-- /#main_sec -->

      <sectionIconBar />
      <!-- /sectionIconBar -->

   </main>
</template>



<style lang="scss" scoped></style>