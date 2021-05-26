<template>

  <b-form @submit.prevent="handleSubmit">
    <b-card
        title="Sign In"
        style="max-width: 45rem; margin-top:50px;"
    >

      <div class="form-group">
        <label>Email address</label>
        <input type="email" v-model="email" class="form-control form-control-lg" />
      </div>

      <div class="form-group">
        <label>Password</label>
        <input type="password" v-model="pass" class="form-control form-control-lg" />
      </div>

      <button type="submit" class="btn btn-dark btn-lg btn-block">Sign In</button>

      <p class="forgot-password text-right mt-2 mb-4">
        <router-link to="/forgot-password">Forgot password ?</router-link>
      </p>

    </b-card>
  </b-form>

</template>

<script>
// @ is an alias to /src


export default {
  name: 'Home',
  data(){
    return{
      email:'',
      pass:'',
    }
  },
  components: {


  },
  methods:{
    handleSubmit(){
      if(this.email && this.pass)
        this.$router.push('/products');
      else
        console.log("fill all fields");
    }
  }
}
</script>

<style>
.card{
  border-radius:15px;
  display: flex;
  text-align: left;
  justify-content: center;
  flex-direction: column;
  width:650px;
}

body{
  
}
</style>
