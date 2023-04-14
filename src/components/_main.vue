<script>

import sectionIconBar from './_iconBar.vue';
import comics from './_comics.vue';

export default {

   name: 'appMain',

   components: {
      sectionIconBar,
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
      <section class="main_jumbo mb-2">
         <div class="tag bg-primary text-white text-uppercase text-center">
            <h4 class="m-0"><strong>current series</strong></h4>
         </div>
      </section>
      <!-- /.main_jumbo -->

      <section id="main_sec">
         <comics />
      </section>
      <!-- /#main_sec -->

      <sectionIconBar />
      <!-- /sectionIconBar -->

   </main>
</template>



<style lang="scss" scoped></style>