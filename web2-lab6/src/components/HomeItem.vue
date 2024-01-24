<script>
export default {
  data() {
    return {
      name: "",
      email: "",
      password:"",
      repeat_password:"",
      welcome_message:""
    }
  },
  methods: {
    register() {
      console.log("An email has been sent to: ", this.email);
    }
  }
}
</script>

<template>
    <h3>
      Please register to access additional features!
    </h3>
    <br>
    <div>Name: <input type="text" placeholder="name" :value="name"></div> 
    <div>Email: <input type="text" placeholder="email" v-model="email"></div>
    <div>Password: <input type="password" placeholder="password" :value="password"></div>
    <div>Repeat password: <input type="password" placeholder="password" :value="repeat_password"></div>

    <button class="btn" type="submit" @click="register">Register</button>
</template>

<style scoped>
  button{
      color: red;
  }
</style>
