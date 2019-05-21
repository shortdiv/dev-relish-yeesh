<template>
  <v-layout row justify-center align-center>
    <v-flex xs12 sm8 md6>
      <StandupForm />
    </v-flex>
  </v-layout>
</template>

<script>
import StandupForm from '../components/StandupForm.vue'
export default {
  components: {
    StandupForm
  }
}
</script>
