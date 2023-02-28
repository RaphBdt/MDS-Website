<script lang="ts">
import { defineComponent } from 'vue'

import Nav from './components/Nav.vue'
import MainTitle from './components/MainTitle.vue'
import Button from './components/Button.vue'
import StudentImages from './components/StudentImages.vue'
import OtherTitles from './components/OtherTitles.vue'
import City from './components/City.vue'

export default defineComponent({
  components: { Nav, MainTitle, Button, StudentImages, OtherTitles, City },
    props: {
        
    },
    setup(props) {
        
    },
    mounted() {
      document.body.classList.add('bg-[#F9FBFC]');
    }
})
</script>


<template>
  <Nav />
  <MainTitle :msg="'La meilleure école des métiers du digital'" />
  <div>
    <Button :text="'Appelez-nous'" />
  </div>
  <StudentImages />
  <OtherTitles type="h3" :msg="'Des campus partout en France'" />
  <City />
  <OtherTitles :type="'h3'" :msg="'Plusieurs spécialités'" />
  <OtherTitles :type="'h2'" :msg="'Les domaines les plus demandés dans le digital'" />
</template>

<style scoped>

</style>
