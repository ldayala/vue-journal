<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <h1>Hola Mundo</h1>
    <button @click="gotTodayBook" class="btn btn-primary">Primary</button>
    <button class="btn btn-secondary">Secundary</button>
    <button class="btn btn-success">Success</button>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  methods:{
    gotTodayBook(){
      this.$router.push({name:'no-entry'});
    }
  }
 
}
</script>
