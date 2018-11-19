<script>
export default {
  name: 'UserSearchForm',
  data() {
    return {
      username: ''
    }
  }
}
</script>

<template>
  <form @submit.prevent="$emit('submitted', username)">
    <label for="male">Git Username: </label>
    <input type="text" v-model="username" id="username" />
    <button type="submit">Submit</button>
  </form>
</template>
