<template>
  <div id="app">
    <div id="navbar-component">
      <b-navbar toggleable="lg" type="dark" variant="dark">
        <b-navbar-brand href="#"><router-link to="/">Icono</router-link></b-navbar-brand>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <!--<router-link to="road">CARRETERA</router-link>-->
            <b-nav-item active><router-link to="road">CARRETERA</router-link></b-nav-item>
            <b-nav-item active href="#">MONTAÑA</b-nav-item>
          </b-navbar-nav>
          <b-navbar-nav class="ml-auto">
            <b-nav-form>
              <b-form-input size="sm" class="mr-sm-2" placeholder="Search"></b-form-input>
              <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
            </b-nav-form>
            <b-nav-item-dropdown right>
              <template v-slot:button-content>
                <em>User</em>
              </template>
              <b-dropdown-item href="#">Profile</b-dropdown-item>
              <b-dropdown-item href="#">Sign Out</b-dropdown-item>
            </b-nav-item-dropdown>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: "App"
};
</script>
<style>
</style>
