<template>
  <v-container fluid>
    <v-layout>
      <v-flex md12 xs12 sm12 class="text-center">
        <v-chip-group dark column>
          <v-chip
            class="ma-2"
            large
            color="black"
            pill
            draggable 
            v-for="lang in items" :key="lang.name">
            <v-avatar>

              <v-img :src="lang.img"></v-img>
            </v-avatar>
            {{ lang.name }}
          </v-chip>
        </v-chip-group>
      </v-flex>
    </v-layout>
  </v-container>

</template>

<script>
  import images from '@/constants/images';

    export default {
      data: () => ({
          items:[
            {
              name:"javascript",
              img:images.javascript
            },
            {
              name:"vue",
              img:images.vue
            },
            {
              name:"html",
              img:images.html
            },
            {
              name:"css",
              img:images.css
            },
            {
              name:"laravel",
              img:images.laravel
            },
            {
              name:"php",
              img:images.php
            },
            {
              name:"java",
              img:images.java
            },
            {
              name:"spring",
              img:images.spring
            },
            {
              name:"mysql",
              img:images.mysql
            },
            {
              name:"mongo",
              img:images.mongo
            },
            {
              name:"wordpress",
              img:images.wordpress
            },
            {
              name:"git",
              img:images.git
            },
            {
              name:"docker",
              img:images.docker
            },
          ]
      }),
    }
</script>

<style lang="css" scoped>
li{
  display: inline;
}
.v-avatar:hover{
  cursor:pointer;
  transform: scale(1.5);
}

</style>