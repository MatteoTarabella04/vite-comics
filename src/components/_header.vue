<script>

import menuLinks from "../assets/data/menuLinks";

export default {

   name: 'appHeader',

   data() {
      return {
         menuLinks,
         activeLink: -1,
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
                  <li v-for="(link, i) in menuLinks" :class="activeLink === i ? 'active' : ''" @click="activeLink = i">
                     <strong><a href="#">{{ link.name.toUpperCase() }}</a></strong>
                  </li>
               </ul>
            </div>
         </div>
      </div>
   </header>
</template>


<style lang="scss" scoped></style>