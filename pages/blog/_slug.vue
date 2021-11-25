<template>
  <article>
    <h1> {{ article.title }} </h1>
    <nuxt-content :document="article" />
    <pre> {{ article }} </pre>
  </article>
</template>

<script>
export default {
  async asyncData ({ $content, params }) {
    // fetch our article here
    const article = await $content('articles', params.slug).fetch()

    return { article }
  }
}
</script>
