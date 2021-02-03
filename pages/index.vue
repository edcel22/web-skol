<template>
  <div id="home" class="default">
    <div class="page_content">
      <section class="technologies">
        <h2>Technologies</h2>
        <div class="items">
          <div class="item" v-for="(technology, key) in technologies">
            <div class="top">
              <div class="overlay">
                <div :class="(type === 'Problems' ? 'left' : 'right')" v-for="(type, key) in technology.types">
                  <nuxt-link to="/">{{type}}</nuxt-link>
                </div>
              </div>
              <img src="/images/wordpress-logo.png" alt="WordPress">
            </div>
            <div class="bottom">
              <p>{{technology.name}}</p>
            </div>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>
<script>
  export default {
    data () {
      return {
        technologies: [
          {
            name: "WordPress",
            types: [
              'Problems', 'Notes']
          },
          {
            name: "Laravel",
            types: [
              'Problems', 'Notes']
          },
          {
            name: "Nuxtjs",
            types: [
              'Problems', 'Notes']
          },
          {
            name: "Vuejs",
            types: [
              'Problems', 'Notes']
          },
          {
            name: "Server Stuffs",
            types: [
              'Problems', 'Notes']
          },
        ]
      }
    }
  }
</script>