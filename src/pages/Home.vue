<template>
  <div class="home">
    <img class="bg" src="../assets/bg.png" alt="" srcset="" />
    <div class="content">
      <p class="page_name">Accueil > <span>facileasimuler</span></p>
      <div class="title_page">
        <img class="logo_2" src="../assets/logo2.jpg" alt="" srcset="" />
        <h1><span>Titre pour la page</span></h1>
        <h1>Facile à simuler à faire</h1>
      </div>
    </div>

    <h2>La gamme de <span>Simulation</span></h2>
  </div>
  
  <div class="grid">
    
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>

    
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>

    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>

    <div class="grid_item">hgxdfhd</div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>

    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>

    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>

    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>
    <div class="grid_item"></div>



  </div>
  
  <div class="contact_bottom">
    <h1>besoin de plus</h1>
    <h1>de renseignement?</h1>
    <a class="contact_button" href=""><button>Nous Contacter</button></a>
  </div>
  <Footer />
</template>


<script>
import Footer from "../components/Footer.vue";
export default {
  name: "Home",
  components: {
    Footer,
  },
};
</script>

<style >
.home {
  text-align: center;
}
span {
  color: #f48d4e;
}
.content {
  box-sizing: border-box;
  background-color: white;
  justify-content: center;
  height: 500px;
  width: 90%;
  top: 290px;
  position: absolute;
  border-radius: 6px;
  left: 5%;
  background-color: #fff;
}
.page_name {
  margin: 20px;
  font-size: 11px;
  position: absolute;
  font-weight: 600;
}

.logo_2 {
  width: 300px;
}

.title_page {
  margin-top: 100px;
  font-size: 35px;
}
h2 {
  margin: 270px;
  font-size: 36px;
  margin-bottom: 100px;
}

.contact_bottom {
  text-align: center;
  box-sizing: border-box;
  background-color: white;
  justify-content: center;
  height: 270px;
  width: 90%;
  top: 125px;
  position: relative;
  border-radius: 0px;
  left: 5%;
  background-color: #fff;
  padding: 60px;
}

.contact_button button {
  margin: 10px;
  background-color: #f48d4e;
  border: none;
  color: white;
  height: 100px;
  height: 48px;
  width: 194px;
  left: 0px;
  top: 0px;
  border-radius: 4px;
  font-weight: 600;
}


.grid {
  max-width: 1300px;
    width: 80%;
    height: auto;
    margin: 30px auto;
    /* border: 1px solid #333; */
    display: grid;
    grid-template-columns: repeat(auto-fill, 300px);
    justify-content: center;
    grid-gap: 10px;
}

.grid_item {
  width: 300px;
    height: 200px;
    background: #fff;
    border-radius: 20px;
}
</style>