<template>
  <div id='login' class='container'>
    <h2>Sign In</h2>
    <form>
      <div class='form-group'>
        <input class='form-control' type='email' placeholder='Email Address' />
        <input class='form-control' type='password' placeholder='Password' />
        <button class='btn'>Sign In</button>
      </div>
    </form>
  </div>
</template>

<script>
  export default {
    created() {
      console.log('login');
    },
  };
</script>
