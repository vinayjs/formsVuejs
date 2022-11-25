<template>
   <forms class="form">
    <div>
      <pre>
        {{JSON.stringify(formValues, null, 2)}}
      </pre>
    </div>
    <div> 
      <label for="name">Name: </label>
      <input type="text" id="name" placeholder="your name" v-model="formValues.name">
    </div>

    <div>
      <label for="'profile">Profile Summary</label>
      <textarea id="profile" />
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
        name: '',
        profileSummary: ''
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
label  {
  font-weight: bold;
  display:flex;
  margin-bottom: 10px;
  margin-top: 10px;
}
input + label{
  display: inline-flex;
  margin-right: 20px;
}
input[type='text'],
textarea,
select{
  display: block;
}
</style>
