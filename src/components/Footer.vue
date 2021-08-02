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
            <li class="services" v-for="service in services" :key="service">{{ service }}</li>
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
        </div>
      </div>
    </div>
    <div class="cpr"></div>
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

ul {
  list-style: none;
  
}
ul li {
  font-size: 15px;
  line-height: 40px;
}

.services {
    font-weight: 400;
}
</style>


