<template>
  <form>
    <label for="fullName">Full Name</label>
    <input type="text" placeholder="FullName..." v-model="fullName">
    <label for="email">Email</label>
    <input type="email" placeholder="Email..." v-model="email">
    <label for="age">Age</label>
    <input type="number" placeholder="Age..." v-model="age">
    <label for="dob">DOB</label>
    <input type="date" placeholder="DOB..." v-model="dob">
    <button type="submit" id="submit" class="border-danger" @click.prevent="submitForm">Submit Form</button>
  </form>
</template>

<script>

export default {
  methods: {
    submitForm(){
      // alert(`${this.fullName} at age ${this.age} was born on ${this.dob} and has an email address of ${this.email}`)
    }
  },
}

</script>
<style scoped>
  form {
    display: flex;
    flex-direction: column;
    width: 80%;
    margin: auto;
  }
  form input{
    margin-bottom: 10px
  }
  form button {
    background-color:crimson;
    color: white;
  }
  form button:hover{
    scale: 1.01
  }
  form button:active{
    scale: 0.99;
  }
</style>