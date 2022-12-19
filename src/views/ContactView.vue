<template>
  <div class="contact">
    <ContactForm/>
  </div>
</template>

<script>
  import ContactForm from "../components/ContactForm.vue"
  export default {
    components:{
      ContactForm
    },
    data() {
      return {
        title: 'Hello',
      }
    }
  }
</script>
<style>
  
</style>