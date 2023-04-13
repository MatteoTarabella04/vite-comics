<script>
export default {

   name: 'sectionIconBar',

   data() {
      return {
         sectionIcons: [
            {
               name: 'digital comics',
               url: 'buy-comics-digital-comics.png',
            },
            {
               name: 'dc merchandise',
               url: 'buy-comics-merchandise.png',
            },
            {
               name: 'subscription',
               url: 'buy-comics-subscriptions.png',
            },
            {
               name: 'comic shop locator',
               url: 'buy-comics-shop-locator.png',
            },
            {
               name: 'dc power visa',
               url: 'buy-dc-power-visa.svg',
            },
         ]
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
               <li v-for="icon in sectionIcons" class="d-flex align-items-center">
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