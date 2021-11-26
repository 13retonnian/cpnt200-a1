/* eslint-disable vue/require-prop-types */
<template>
  <v-container class="flex justify-center align-center flex-col text-center p-10 bg-yellow-200">
    <p class="text-xl text-gray-600">
      &copy; {{footerPage.author}} || MIT License
    </p>
  </v-container>
</template>
<script>
export default {
  // eslint-disable-next-line vue/require-prop-types
  props: ['footerPage']
}
</script>
