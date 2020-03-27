<template>
<nav>
  <div class="navbar desktop">
    <div class="col-left">
      <h1 class="logo">Shaolink</h1>
      <h2 class="nav-link">Features</h2>
      <h2 class="nav-link">Pricing</h2>
      <h2 class="nav-link">Resources</h2>
    </div>
    <div class="col-right">
      <h2 class="login-link">Login</h2>
      <button class="sign-button" type="button">Sign Up</button>
    </div>
  </div>
  <div class="navbar mobile">
    <div class="col-left">
      <h1 class="logo">Shaolink</h1>
    </div>
    <div class="col-right">
      <img :src="require('@/assets/menu.svg')" alt="Menu icon" @click="collapsed = !collapsed">
    </div>
  </div>
  <div v-show="collapsed" class="col-bottom">
    <h2 class="nav-link">Features</h2>
    <h2 class="nav-link">Pricing</h2>
    <h2 class="nav-link">Resources</h2>
    <hr>
    <h2 class="login-link">Login</h2>
    <button class="sign-button" type="button">Sign Up</button>
  </div>
</nav>
</template>

<script>
export default {
  name: 'Navbar',
  data () {
    return {
      collapsed: false
    }
  }
}
</script>
