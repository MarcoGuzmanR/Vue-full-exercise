<template>
  <div id='register' class='container'>
    <h2>Register Form</h2>
    <input class='form-control' placeholder='First Name' />
    <input class='form-control' placeholder='Last Name' />
    <input class='form-control' placeholder='Email Address' />
    <input class='form-control' placeholder='Pick a Password' />
    <input class='form-control' placeholder='Confirm Password' />
    <button class='btn'>Sign Up</button>

    <famous></famous>
  </div>
</template>

<script>
  import Famous from './Famous';

  export default {
    components: {
      Famous,
    },
    created() {
      console.log('register');
    },
  };
</script>
