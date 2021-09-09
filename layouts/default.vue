<template>
    <v-app>
      <div class="d-flex flex-column">
        <div><Core-Nav/></div>
        <div class="w-screen"><Nuxt/></div>
        <div class=" "><Core-Footer/></div>
      </div>
    </v-app>

</template>

<script>
export default {

}
</script>

<style>
::-webkit-scrollbar {
  display: none;
}
 
/* #app{
  margin: 0;
  padding: 0;
}

.Nav{
  height: 15%;
} */
</style>