<template>
  <div>
    <Header :headerPage="info" />
    <h1 class="text-7xl p-10 text-center">
      Castles
    </h1>
    <nuxt-img class="block ml-auto mr-auto w=3/6" src="/castle1.jpg" />
    <nuxt-img class="block ml-auto mr-auto w-3/6" src="/castle2.jpg" />
    <NuxtLink class="text-7xl p-10 text-center text-blue-900 block" to="/">
      Click here for amazing hilarious jokes
    </NuxtLink>
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
