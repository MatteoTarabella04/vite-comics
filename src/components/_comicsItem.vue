<script>
export default {

   name: 'comicsItem',

   props: {
      thumb: String,
      price: String,
      series: String,
      type: String,
   }

}
</script>
<template>
   <div class="col">
      <div class="item">
         <img :src="thumb" :alt="series">
         <div class="desc text-white py-3 text-uppercase">
            <span>{{ series }}</span>
         </div>
      </div>
   </div>
</template>


<style lang="scss" scoped></style>