<template>
  <div id="app">
    <router-view />
  </div>
</template>

<script>
// remember to npm install sass-loader node-sass --save-dev to prevent error
// https://webpack.docschina.org/loaders/sass-loader/
import '@/assets/stylesheets/main.scss'

export default {
  name: 'App'
}
</script>
