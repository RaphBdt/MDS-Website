<script lang="ts">
import { defineComponent } from 'vue'

import Container from './components/Container.vue'
import Nav from './components/Nav.vue'
import MainTitle from './components/MainTitle.vue'
import Button from './components/Button.vue'
import StudentImages from './components/StudentImages.vue'
import OtherTitles from './components/OtherTitles.vue'
import City from './components/City.vue'
import Category from './components/Category.vue'
import Point from './components/Point.vue'
import ArticleCard from './components/ArticleCard.vue'
import Arrow from './components/Arrow.vue'
import Alumni from './components/Alumni.vue'
import Newsletter from './components/Newsletter.vue'

export default defineComponent({
  components: { Nav, MainTitle, Button, StudentImages, OtherTitles, City, Category, Point, ArticleCard, Container, Arrow, Alumni, Newsletter },
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
  <OtherTitles class="text-center" type="h3" msg="Des campus partout en France" />
  <City class="mt-8 mb-[170px]" numberOfStudents="2000" imageFile="ville1.png" />
  <OtherTitles class="text-center" type="h3" msg="Plusieurs spécialités" />
  <OtherTitles class="w-[600px] mx-auto mt-4 text-center" type="h2" msg="Les domaines les plus demandés dans le digital" />
  <div class="relative">
    <Container>
      <div class="flex justify-around align-center mt-24">
        <Category title="Webmarketing" description="Classée la 2ème meilleure école de France dans ce domaine, le marketing digital est la spécialité de MyDigitalSchool" />
        <Category title="UI & UX Design" description="Classée la 2ème meilleure école de France dans ce domaine, le marketing digital est la spécialité de MyDigitalSchool" />
        <Category title="Programmation" description="Classée la 2ème meilleure école de France dans ce domaine, le marketing digital est la spécialité de MyDigitalSchool" />
        <Category title="Communication" description="Classée la 2ème meilleure école de France dans ce domaine, le marketing digital est la spécialité de MyDigitalSchool" />
      </div>
    </Container>
    <Point class="absolute left-[250px] -top-[150px]" color="primary" size="medium" />
    <Point class="absolute right-[180px] -top-[120px]" color="secondary" size="big" />
  </div>
  <div class="flex justify-center mt-[50px]">
    <Button class="mx-auto mt-8" text="Télécharger le programme" />
  </div>
  <div class="bg-[#181B3F] w-full my-32 pt-10 pb-32">
    <OtherTitles class="w-[600px] mx-auto text-white my-20 text-center" type="h2" msg="MyDigitalSchool, c'est aussi un blog avec des conseils" />
    <Container>
      <div class="flex justify-around align-center">
        <ArticleCard img="blog1.jpg" date="4 mars" title="Comment devenir développeur web ?" />
        <ArticleCard img="blog2.jpg" date="5 avril" title="UX vs UI Design, quelle est la différence ?" />
        <ArticleCard img="blog3.jpg" date="9 avril" title="Top 10 des métiers du digital en 2023" />
        <ArticleCard img="blog1.jpg" date="4 mars" title="Comment devenir développeur web ?" />
      </div>
    </Container>
  </div>
  <Container>
    <div class="flex justify-between items-center">
      <OtherTitles class="w-[400px] mt-4" type="h2" msg="Qu'est-ce que nos alumnis en pensent ?" />
      <div class="flex">
        <Arrow class="mr-5" direction="left" />
        <Arrow direction="right" />
      </div>
    </div>
  </Container>
  <Container>
    <div class="flex justify-between mt-20">
      <Alumni class="w-[47%]" img="alumni1.jpg" firstname="Mélanie" promotion="Étudiante en 2015" description="J’ai passé clairement mes 2 meilleurs années scolaires à MyDigitalSchool. L’ambiance, les intervenants et les locaux m’ont permis de m’épanouir, gros big up pour la connexion internet ! ❤️" date="Mars 2022" />
      <Alumni class="w-[47%]" img="alumni2.jpg" firstname="Léo" promotion="Étudiant en 2015" description="J’ai passé clairement mes 2 meilleurs années scolaires à MyDigitalSchool. L’ambiance, les intervenants et les locaux m’ont permis de m’épanouir, gros big up pour la connexion internet ! ❤️" date="Juin 2017" />
    </div>
  </Container>
  <Container>
    <Newsletter class="mt-40" />
  </Container>
</template>

<style scoped>

</style>
