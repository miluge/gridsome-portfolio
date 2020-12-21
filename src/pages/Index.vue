<template>
  <Layout>
    <!-- Intro -->
    <section>
      <div class="h-screen flex justify-center items-center">
        <h1 class="text-6xl">Guillaume Blondel</h1>
      </div>
      <p class="bg-white dark:bg-black">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Pariatur excepturi labore tempore expedita, et iste tenetur suscipit explicabo! Dolores, aperiam non officia eos quod asperiores
      </p>
    </section>
    <!-- Projects -->
    <section>
      <h2>Projects</h2>
    </section>
    <!-- Projects -->
    <slider/>
    <!-- Get in touch! -->
    <section>
      <div class="max-w-md flex justify-center">
        <h3 class="text-2xl">Get in touch</h3>
        <p>
          <a class="text-9xl">Gllmblndl@gmail.com</a>
        </p>
      </div>
    </section>
    
  </Layout>
</template>

<script>
import Slider from "../components/Slider";
export default {
  components: {Slider},
  metaInfo: {
    title: 'Hello, world!'
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
