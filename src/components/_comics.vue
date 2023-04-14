<script>

import comicsList from '../assets/data/dc-comics.json';
import comicsItem from './_comicsItem.vue';

export default {
   name: 'comics',

   components: {
      comicsItem,
   },

   data() {
      return {
         comicsList,
      }
   }
}
</script>

<template>
   <div class="container p-5">
      <div class="row row-cols-6">
         <comicsItem v-for="item in comicsList" :thumb="item.thumb" :series="item.series" />
      </div>
      <div class="load_btn w-100 d-flex justify-content-center">
         <button class="btn text-uppercase bg-primary text-white rounded-0 px-5"><strong>load more</strong></button>
      </div>
   </div>
</template>


<style lang="scss" scoped></style>