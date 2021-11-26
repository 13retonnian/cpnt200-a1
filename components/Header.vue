<template>
  <div class="flex justify-center align-center flex-col text-center p-10 bg-yellow-200">
    <h1 class="p-5 text-5xl font-bold">
      {{ headerPage.title }}
    </h1>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/require-prop-types
  props: ['headerPage']
}
</script>
