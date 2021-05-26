<template>
  <b-navbar toggleable="sm" type="light" variant="light">
    <b-navbar-toggle target="nav-text-collapse"></b-navbar-toggle>

    <b-navbar-brand>Transcontinental</b-navbar-brand>

    <b-collapse id="nav-text-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item to="/">Login</b-nav-item>
         <b-nav-item to="/" v-show=false>Logout</b-nav-item>

      
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
export default {
    data(){
      return{
        
      }
    },
 
}
</script>

<style scoped>

</style>
