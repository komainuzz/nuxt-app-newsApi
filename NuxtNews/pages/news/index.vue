<template>
  <div>
    aaaaaaa
  </div>
</template>

<script>
const URL =
  'http://newsapi.org/v2/top-headlines?country=jp&apiKey=5d5848681ac64598adaa5be9de67ea6d'

export default {
  async ascyncData({ app }) {
    const news = await app.$axios.$get(URL)
    console.log(news)
    console.log('hi')
  }
}
</script>
