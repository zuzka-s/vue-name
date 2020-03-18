<template>
  <div>
    <p>
      first name:
      <input v-model="editableName" />
    </p>
    <p>
    </p>
     <p>
      last name:
      <input v-model="editableLastName" />
    </p>
    <p>
      {{ editableName }} {{ editableLastName }}
    </p>
  </div>
</template>

<script>
export default {
  name: 'NameEditor',
  data () {
    return {
      editableName: this.firstName,
      editableLastName: this.lastName
    }
  },
  props: {
    firstName: {
      type: String,
      default: 'John'
    },
    lastName: {
      type: String,
      default: 'Doe'
    }
  }
}
</script>

<style scoped>

</style>
