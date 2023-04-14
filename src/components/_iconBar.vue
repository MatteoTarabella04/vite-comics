<script>

import iconBar from "../assets/data/iconBar";

export default {

   name: 'sectionIconBar',

   data() {
      return {
         iconBar,
      }
   },
   methods: {
      getImgPath(imgPath) {
         return new URL(imgPath, import.meta.url).href;
      }
   }
}
</script>
<template>
   <section id="icon_sec" class="bg-primary">
      <div class="container h-100">
         <div class="content h-100 d-flex justify-content-center align-items-center">
            <ul class="list-unstyled d-flex m-0 gap-5">
               <li v-for="icon in iconBar" class="d-flex align-items-center">
                  <img :src="getImgPath(`../assets/img/${icon.url}`)" :alt="icon.name" height="55">
                  <a href="#" class="ps-3">{{ icon.name.toUpperCase() }}</a>
               </li>
            </ul>
         </div>
      </div>
      <!-- /.container -->
   </section>
   <!-- /#icon_sec -->
</template>


<style lang="scss" scoped></style>