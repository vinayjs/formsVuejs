<template>
   <forms>
    <div> 
      <label for="name">Name : </label>
      <input type="text" id="name">
    </div>
   </forms>

</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      formValues: {
        name: ''
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}

</style>
