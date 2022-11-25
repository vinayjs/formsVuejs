<template>
   <forms>
    <div>
      <pre>
        {{JSON.stringify(formValues, null, 2)}}
      </pre>
    </div>
    <div> 
      <label for="name">Name: </label>
      <input type="text" id="name" placeholder="your name" v-model="formValues.name">
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
label  {
  font-weight: bold;
  display:inline-flex;
  margin-bottom: 5px;
}
input {
  position: flex
}

</style>
