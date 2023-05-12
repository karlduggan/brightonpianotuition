<template>
  <div class="bg-[#7a8a61]">
    <div class="h-screen">
      <div class="container mx-auto max-w-screen-xl">
        <HeadderComponent></HeadderComponent>
        <HeroComponent></HeroComponent>
      </div>
    </div>
    <div class="h-screen">
      <AboutComponent></AboutComponent>
    </div>
    <div class="h-screen">
      <LessonComponent></LessonComponent>
    </div>
    <div class="h-screen">
      <ContactComponent></ContactComponent>
    </div>
    <FooterComponent></FooterComponent>
  </div>


</template>
<script>
import HeroComponent from './components/HeroComponent.vue';
import HeadderComponent from './components/HeaderComponent.vue'
import AboutComponent from './components/AboutComponent.vue'
import LessonComponent from './components/LessonComponent.vue'
import ContactComponent from './components/ContactComponent.vue'
import FooterComponent from './components/FooterComponent.vue'

export default {
  name: 'App',
  components: {
    HeroComponent,
    HeadderComponent,
    AboutComponent,
    LessonComponent,
    ContactComponent,
    FooterComponent
  }
}
</script>

<style>

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
