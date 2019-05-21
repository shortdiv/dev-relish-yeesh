<template>
  <div>
    <v-form>
      <v-text-field v-model="form.firstName" label="First name*"></v-text-field>
      <v-text-field
        v-model="form.lastWeek"
        label="What did you work on last week?*"
      ></v-text-field>
      <v-text-field
        v-model="form.thisWeek"
        label="What are you going to focus on this week?*"
      >
      </v-text-field>
      <v-text-field
        v-model="form.topics"
        label="Are there any main topics would you like to address this week?"
      ></v-text-field>
      <v-text-field
        v-model="funThings"
        label="Anything fun to share?"
      ></v-text-field>
      <v-card-actions class="justify-center">
        <v-btn depressed large @click="update">
          Submit
        </v-btn>
      </v-card-actions>
    </v-form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        firstName: null,
        lastWeek: null,
        thisWeek: null,
        topics: null,
        funThings: null
      }
    }
  },
  methods: {
    submit() {
      console.log('submit!')
    }
  }
}
</script>

<style lang="scss" scoped></style>
