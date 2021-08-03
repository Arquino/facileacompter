<template>
  <div class="footer">
    <div class="contact_footer">
      <img
        class="logo_footer"
        src="../assets/logo_footer.jpg"
        alt=""
        srcset=""
      />
    </div>
    <div class="content_footer">
      <div class="row_footer">
        <div class="col_footer">
          <h4>
            Facilacompter, pour simplifier votre comptabilité et la gestion de
            votre entreprise.
          </h4>
        </div>
        <div class="col_footer">
          <h4>SERVICES</h4>
          <ul>
            <li class="services" v-for="service in services" :key="service">
              {{ service }}
            </li>
          </ul>
        </div>
        <div class="col_footer">
          <h4>NOUS SUIVRE</h4>
          <ul>
            <li class="socials" v-for="social in socials" :key="social">
              {{ social }}
            </li>
          </ul>
        </div>
        <div class="col_footer">
          <h4>NOUS CONTACTER</h4>
          <p class="info">Info@facilacompter.com</p>
          <p class="info">04 94 10 87 30</p>
          <p class="info">
            111 Chemin des Négadoux <br />
            83140 Six-Fours les Plages
          </p>
        </div>
      </div>
    </div>
    <div class="cpr">
      <p>
        Facilacompter® est une marque déposée par Christelle Ouvrard, du Groupe
        Fiducie Audit et Conseil®.
      </p>
      <div class="nav_footer">
        <ul>
          <li>Qui sommes-nous</li>
          <li>Mention légale</li>
          <li>CGV</li>
          <li>CGU</li>
        </ul>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: "Footer",
  components: {},
  data() {
    return {
      services: [
        "Facilapaie",
        "Facilafacturer",
        "Facilagérer",
        "Facilapiloter",
        "Facilaformer",
        "Facilastocker",
        "Autres",
        "services",
      ],
      socials: ["Facebook", "Linkedin"],
    };
  },
};
</script>

<style>
.footer {
  padding: 50px;
  background-color: #19191b;
  color: white;
  height: auto;
}
.logo_footer {
  height: 30px;
  margin-bottom: 30px;
  margin-top: 100px;
  margin-left: 100px;
}

.content_footer {
  /* display: flex; */
  /* text-align: center; */
  justify-content: center;
}
.row_footer {
  display: flex;
  justify-content: space-between;
}

.col_footer {
  width: 600px;
  margin-right: 100px;
  padding-left: 100px;
}
.col_footer h4 {
  margin-bottom: 15px;
}
.col_footer .info {
  margin-top: 25px;
}

ul {
  list-style: none;
}
ul li {
  font-size: 15px;
  line-height: 32px;
}

.services {
  font-weight: 400;
}
.socials {
  text-decoration: underline;
}
.cpr {
  display: flex;
  justify-content: space-between;
}
.cpr p {
  margin-top: 70px;
  width: 312px;
  font-size: 10px;
}

.nav_footer ul {
  display: flex;
  margin-top: 50px;
  font-size: 10px;
}
.nav_footer ul li {
  display: flex;
  margin-top: 60px;
  font-size: 10px;
  margin: 15px;
}
</style>


