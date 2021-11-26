<template>
  <div>
    <Header :headerPage="info" />
    <NuxtLink to="/">First Page</NuxtLink>
    <nuxt-img src="/castle2.jpg" />
    <Footer :footerPage="info" />
  </div>
</template>

<script>
export default {
  data () {
    return {
      script: [
        { src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }
      ],
      info: {
        title: 'Jokes and Castles',
        description: 'Jokes and Castles',
        author: 'Christopher Barber',
        license: 'MIT License'
      }
    }
  }
}
</script>
