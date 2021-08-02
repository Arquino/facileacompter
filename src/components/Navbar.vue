<template>
  <img class="logo" src="../assets/logo.jpg" alt="logo" srcset="" />
  <nav>
    <ul class="nav_links">
      <li><a href="#">Nos solution</a></li>
      <li><a href="#">Autres services</a></li>
      <li><a href="#">Qui sommes-nous?</a></li>
    </ul>
  </nav>
  <div registration_demo>
    <a class="login" href="">connexion</a>
    <a class="demo" href=""><button>Demander une démo</button></a>
  </div>
</template>


<script>
  export default {
    name: "navbar",
  };
</script>


<style>
/* @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100&display=swap'); */
    /* @import url("https://fonts.googleapis.com/css2?family=Inter:wght@600&display=swap"); */
    .logo {
      left: 0px;
      width: 250px;
      height: 40px;
    }
    a button {
      text-decoration: none;
    }
    nav {
      display: flex;
      text-align: center;
      /* margin: auto; */
      margin-left: 100px;
    }
    nav .nav_links {
      list-style: none;
      font-style: normal;
      font-weight: 600;
      font-size: 16px;
      line-height: 19px;
      margin-left: 30px;
      margin-right: 30px;
    }

    nav .nav_links li a {
      transition: all 0.3s ease 0s;
      text-decoration: none;
      color: black;
    }
    nav .nav_links li {
      display: inline-block;
      text-decoration: none;
      color: black;
      padding: 10px;
    }

    div .registration_demo {
      display: flex;
      justify-content: space-between;
    }

    .login {
      text-decoration: none;
      color: #f48d4e;
      margin-right: 20px;
      font-weight: 600;
    }

    .demo button {
      font-weight: 600;
      background-color: #f48d4e;
      border: none;
      color: white;
      height: 100px;
      height: 48px;
      width: 194px;
      left: 0px;
      top: 0px;
      border-radius: 4px;
    }
</style>