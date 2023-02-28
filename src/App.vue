<script lang="ts">
import { defineComponent } from 'vue'

import Nav from './components/Nav.vue'
import MainTitle from './components/MainTitle.vue'
import Button from './components/Button.vue'
import StudentImages from './components/StudentImages.vue'
import OtherTitles from './components/OtherTitles.vue'
import City from './components/City.vue'
import Category from './components/Category.vue'
import Point from './components/Point.vue'

export default defineComponent({
  components: { Nav, MainTitle, Button, StudentImages, OtherTitles, City, Category, Point },
    props: {
        message: String
    },
    setup(props) {
        
    },
    mounted() {
      document.body.classList.add('bg-[#F9FBFC]');
    }
})
</script>


<template>
  <Nav class="my-14" />
  <MainTitle class="w-[600px] mx-auto mt-30" msg="La meilleure école des métiers du digital" />
  <div class="flex justify-center">
    <Button class="mx-auto mt-8" text="Appelez-nous" />
  </div>
  <StudentImages class="mx-auto my-36" />
  <OtherTitles type="h3" msg="Des campus partout en France" />
  <City class="mt-8 mb-[170px]" numberOfStudents="2000" imageFile="ville1.png" />
  <OtherTitles type="h3" msg="Plusieurs spécialités" />
  <OtherTitles class="w-[600px] mx-auto mt-4" type="h2" msg="Les domaines les plus demandés dans le digital" />
  <div class="relative">
    <div class="container mx-auto flex justify-around align-center mt-24">
      <Category title="Webmarketing" description="Classée la 2ème meilleure école de France dans ce domaine, le marketing digital est la spécialité de MyDigitalSchool" />
      <Category title="UI & UX Design" description="Classée la 2ème meilleure école de France dans ce domaine, le marketing digital est la spécialité de MyDigitalSchool" />
      <Category title="Programmation" description="Classée la 2ème meilleure école de France dans ce domaine, le marketing digital est la spécialité de MyDigitalSchool" />
      <Category title="Communication" description="Classée la 2ème meilleure école de France dans ce domaine, le marketing digital est la spécialité de MyDigitalSchool" />
    </div>
    <Point class="absolute left-[250px] -top-[150px]" color="primary" size="medium" />
    <Point class="absolute right-[180px] -top-[120px]" color="secondary" size="big" />
  </div>
  <div class="flex justify-center mt-[50px]">
    <Button class="mx-auto mt-8" text="Télécharger le programme" />
  </div>
</template>

<style scoped>

</style>
