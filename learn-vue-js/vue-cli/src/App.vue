<template>
  <div>
    <app-header v-bind:propsdata="str"
                v-on:renew="renewStr"></app-header>
  </div>
</template>

<script>
import AppHeader from "@/components/AppHeader";

export default {
  data() {
    return {
      str: 'Header'
    }
  },
  components: {
    'app-header': AppHeader
  },
  methods: {
    renewStr(){
      this.str = 'hi'
    }
  }
}
</script>

<style scoped>

</style>