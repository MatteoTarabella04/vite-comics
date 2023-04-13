<script>
export default {

   name: 'appHeader',

   data() {
      return {
         menuLinks: [
            {
               name: "characters",
            },
            {
               name: "comics",
            },
            {
               name: "movies",
            },
            {
               name: "tv",
            },
            {
               name: "games",
            },
            {
               name: "collectibles",
            },
            {
               name: "videos",
            },
            {
               name: "fans",
            },
            {
               name: "news",
            },
            {
               name: "shop",
            },
         ]
      }
   }

}
</script>
<template>
   <header>
      <div class="container">
         <div class="nav d-flex justify-content-between align-items-center">
            <div class="logo p-3">
               <a href="/">
                  <img src="../assets/img/dc-logo.png" alt="dc_logo" width="80">
               </a>
            </div>
            <div class="menu">
               <ul class="list-unstyled d-flex gap-4 mb-0">
                  <li v-for="link in menuLinks">
                     <strong><a href="#">{{ link.name.toUpperCase() }}</a></strong>
                  </li>
               </ul>
            </div>
         </div>
      </div>
   </header>
</template>


<style lang="scss" scoped></style>