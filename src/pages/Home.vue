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
    <div class="grid_item secteur" v-for="secteur in secteurs" :key="secteur">
      <img class="round_logo" src="../assets/logo_round.png" alt="" srcset="" />
      <h5>{{ secteur }}</h5>
    </div>

    <div class="grid_item title_row">Vos besoins et objectifs</div>
    <div
      class="grid_item objectif"
      v-for="objectif in objectifs"
      :key="objectif"
    >
      <h5>vous souhaitez <br /></h5>
      <span>{{ objectif }}</span>
    </div>

    <div class="grid_item title_row"> Nos conseils et recommandations du PÔLE CONSEIL</div>
    <div class="grid_item conseil"> 
       <p>Vous obtenez après la prise de connaissance des données utiles :</p>  <br>
        <p>1. La connaissance de votre niveau d’imposition</p>  <br>
        <p>  2. <span>La déclaration de revenu</span> par l’intermédiaire <span> d’un tiers de confiance</span> votre <span> expert-comptable.</span></p> <br>
    </div>
    <div class="grid_item conseil"> 
       <p>Vous obtenez après la prise de connaissance des données utiles :</p>  <br>
        <p>1. La connaissance de votre niveau d’imposition</p>  <br>
        <p>  2. <span>La déclaration de revenu</span> par l’intermédiaire <span> d’un tiers de confiance</span> votre <span> expert-comptable.</span></p> <br>
    </div>
    <div class="grid_item conseil"> 
       <p>Vous obtenez après la prise de connaissance des données utiles :</p>  <br>
        <p>1. La connaissance de votre niveau d’imposition</p>  <br>
        <p>  2. <span>La déclaration de revenu</span> par l’intermédiaire <span> d’un tiers de confiance</span> votre <span> expert-comptable.</span></p> <br>
    </div>
    <div class="grid_item conseil"> 
       <p>Vous obtenez après la prise de connaissance des données utiles :</p>  <br>
        <p>1. La connaissance de votre niveau d’imposition</p>  <br>
        <p>  2. <span>La déclaration de revenu</span> par l’intermédiaire <span> d’un tiers de confiance</span> votre <span> expert-comptable.</span></p> <br>
    </div>

    <div class="grid_item title_row">Les livrables du PÔLE CONSEIL</div>
    <div
      class="grid_item livrable"
      v-for="livrable in livrables"
      :key="livrable"
    >
      <ul>
        <li>{{ livrable.a }}</li>
        <li>{{ livrable.b }}</li>
        <center>
          <li>{{ livrable.e }}</li>
        </center>
        <center>
          <li>{{ livrable.e }}</li>
        </center>
      </ul>
    </div>
    <div
      class="grid_item livrable"
      v-for="livrable in livrables"
      :key="livrable"
    >
      <ul>
        <li>{{ livrable.a }}</li>
        <li>{{ livrable.b }}</li>
        <center>
          <li>{{ livrable.e }}</li>
        </center>
        <center>
          <li>{{ livrable.e }}</li>
        </center>
      </ul>
    </div>
    <div
      class="grid_item livrable"
      v-for="livrable in livrables"
      :key="livrable"
    >
      <ul>
        <li>{{ livrable.c }}</li>
        <li>{{ livrable.d }}</li>
        <li>{{ livrable.b }}</li>
      </ul>
    </div>
    <div
      class="grid_item livrable"
      v-for="livrable in livrables"
      :key="livrable"
    >
      <ul>
        <li>{{ livrable.c }}</li>
        <li>{{ livrable.d }}</li>
        <li>{{ livrable.b }}</li>
      </ul>
    </div>

    <div class="grid_item title_row">Nos tarif</div>
    <div class="grid_item tarif" v-for="tarif in tarifs" :key="tarif">
      {{ tarif }}
    </div>

    <div class="grid_item title_row">
      Les services associés <span>Bénéficiez d’un crédit d’impôt de 50%*</span>
    </div>
    <div class="grid_item service" v-for="service in services" :key="service">
      <img class="icon" v-bind:src="service.check" alt="" srcset="" />
    </div>
    <div class="grid_item service" v-for="service in services" :key="service">
      <img class="icon" v-bind:src="service.check" alt="" srcset="" />
    </div>
    <div class="grid_item service" v-for="service in services" :key="service">
      <img class="icon" v-bind:src="service.check" alt="" srcset="" />
    </div>
    <div class="grid_item service" v-for="service in services" :key="service">
      <img class="icon" v-bind:src="service.time" alt="" srcset="" />
    </div>

    <div class="grid_item"></div>
    <div class="grid_item talk"><button>Parlons-en</button></div>
    <div class="grid_item talk"><button>Parlons-en</button></div>
    <div class="grid_item talk"><button>Parlons-en</button></div>
    <div class="grid_item talk"><button>Parlons-en</button></div>
  </div>


  <div class="condition">
    <h3>*Demandez les conditions d’éligibilité</h3>
    <p>Votre expert-comptable en étant adhérent à la coopérative Hexa Coop bénéficie de l’agrément préfectoral de services à domicile de la 
      coopérative. Ce dispositif vous
       permet de bénéficier de 50% de crédit d’impôt sur certaines prestations dans certaines conditions.</p>
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
import check from "../assets/check.png";
import time from "../assets/time-real.png";
export default {
  name: "Home",
  components: {
    Footer,
  },
  data() {
    return {
      secteurs: [
        "immobilier",
        "Automobile",
        "impôt sur revenu",
        "cotisatio non salariés",
      ],

      objectifs: [
        "optimiser l’acquisition d’un investissement immobilier ?",
        "optimiser l’acquisition d’un véhicule (tourisme ou utilitaire) ?",
        "optimiser, simuler et déclarer votre imposition sur le revenu",
        "optimiser, simuler et déclarer cotisations sociales en tant qu’Indépendant ?",
      ],
      conseils: [],
      livrables: [
        {
          a: "Un rapport détaillé",
          b: "Un compte rendu",
          c: "La signature d’un tiers de confiance",
          d: "Un document de synthèse",
          e: "-",
        },
      ],
      tarifs: [
        "En fonction du temps passé de 500 € HT à 2500 € HT",
        "Forfait de 350 € HT",
        "En fonction du temps passé de 100 € HT à 800 € HT",
        "Forfait de 350 € HT",
      ],
      services: [
        {
          check: check,
          time: time,
        },

        // 'fa-check-circle',
        // 'fa-check-circle',
        // 'fa-check-circle',
        // 'fa-fa-times-circle',
      ],
    };
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
  grid-template-columns: repeat(auto-fill, 200px);
  justify-content: center;
  grid-gap: 10px;
}

.grid_item {
  width: 300px;
  height: 118px;
  /* background: #333; */
  /* border-radius: 20px; */
  text-align: center;
}

.secteur {
  display: flex;
  width: 200px;
  height: 80px;
  color: black;
  background-color: #fff;
  border-radius: 5px;
  text-align: left;
}

.title_row {
  padding: 30px;
  text-align: start;
  font-weight: 700;
  width: auto;
}
.round_logo {
  width: 50px;
  height: 50px;
  margin-top: 24px;
  margin-left: 15px;
  margin: 15px;
}

.secteur h5 {
  margin-top: 22px;
}

.objectif {
  background-color: #fff;
  color: #f48d4e;
  font-weight: 600;
  text-align: left;
  padding: 10px;
  width: auto;
  height: auto;
  border-radius: 5px;
}
.objectif h5 {
  color: #19191b;
  font-size: 16px;
}
.objectif span {
  font-size: 15px;
}

.conseil {
  background-color: #fff;
  color: #1e1f20;
  font-weight: 600;
  text-align: left;
  padding: 10px;
  width: auto;
  height: auto;
  border-radius: 5px;
}
.conseil p {
  font-weight: 400;
}

.livrable {
  text-align: left;
  background-color: #fff;
  padding: 20px;
  color: #1e1f20;
  width: 200px;
  height: auto;
  font-weight: 600;
  border-radius: 5px;
}
.livrable ul li {
  list-style-type: disc;
  line-height: 1;
  margin: 10px;
}

.tarif {
  text-align: center;
  background-color: #fff;
  height: auto;
  padding: 20px;
  font-weight: 600;
  font-size: 16px;
  width: 200px;
  color: #555555;
  border-radius: 5px;
}

.service {
  text-align: center;
  background-color: #fff;
  height: auto;
  padding: 20px;
  font-weight: 600;
  font-size: 16px;
  width: 200px;
  color: #555555;
  border-radius: 5px;
}
.talk {
  text-align: center;
  height: 90px;
  padding: 20px;
  font-weight: 600;
  font-size: 16px;
  width: 200px;
  color: #555555;
  border-radius: 5px;
}
.icon {
  margin-top: 11px;
  width: 50px;
  height: 50px;
}

.talk button {
  background-color: #f48d4e;
  width: 100px;
  height: 50px;
  border: none;
  color: white;
  font-weight: 600;
  border-radius: 5px;
}

.condition {
  padding: 20px
}
.condition h3 {
  padding: 15px;
  margin-bottom: -20px;
}
.condition  p {
  padding: 20px;
  font-size: 18px;
  font-weight: 400;
  font-style: normal;
}
</style>