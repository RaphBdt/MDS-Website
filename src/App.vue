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
  <City class="mt-8" numberOfStudents="2000" imageFile="ville1.png" />
</template>

<style scoped>

</style>
