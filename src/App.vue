<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <Suspense>
    <template #default>
      <Users />
    </template>
    <template #fallback>
      <div>Loading...</div>
    </template>
  </Suspense>
  <SecondaryUsage />
</template>

<script>
import Users from './components/Users'
import SecondaryUsage from "./components/SecondaryUsage.vue";

export default {
  name: 'App',
  setup () {

  },
  components: {
    Users,
    SecondaryUsage
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
