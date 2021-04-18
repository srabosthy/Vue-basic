<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item active">
            <router-link class="nav-link" to="/">Home<span class="sr-only">(current)</span></router-link>
          </li>
          <li class="nav-item">
            <li class="nav-item"> <router-link class="nav-link" to="/about-us">About</router-link>
          </li>
          <li class="nav-item">
            <li class="nav-item"> <router-link class="nav-link" to="/history">History</router-link>
          </li>
          <li class="nav-item">
            <li class="nav-item"> <router-link class="nav-link" to="/team">Team</router-link>
          </li>
          <li class="nav-item">
            <li class="nav-item"> <router-link class="nav-link" to="/parent">Parent</router-link>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
              Manage
            </a>
            <div class="dropdown-menu" aria-labelledby="navbarDropdown">
              <router-link class="nav-link" to="/manage-product">Manage Product</router-link>
              <div class="dropdown-divider"></div>
              <router-link class="nav-link" to="/manage-product/product">Product List</router-link>
              <router-link class="nav-link" to="/manage-product/create">Create-Product</router-link>
            </div>
          </li>
        </ul>
        <form class="form-inline my-2 my-lg-0">
          <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
        </form>
      </div>
    </nav>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}
</style>
