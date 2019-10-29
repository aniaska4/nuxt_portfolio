<template>
  <div>
    <Nav/>
    <Title/>
    <About/>
    <Skills/>
    <Projects/>
    <nuxt />
  </div>
</template>

<script>
import Nav from './main/Nav'
import Title from './main/Title'
import About from './main/About'
import Skills from './main/Skills'
import Projects from './main/Projects'
export default {
    name: 'default',
    components: {     
      Nav,
      Title,
      About,
      Skills,
      Projects
}
}

</script>


<style>
body { font-family: 'EB Garamond', serif, 'Times New Roman', serif; height: 100%; width: 100%; }

* { margin: 0; padding: 0; box-sizing: border-box; }

.container { max-width: 1200px; width: 100%; margin: 0 auto; }

</style>
