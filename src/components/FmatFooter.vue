<template lang="html">
  <div class="footer">
    <div class="contacto">
      <h2>Contacto</h2>
      <p><strong>Dirección:</strong> <br> Anillo Periférico Norte, Tablaje Cat. 13615, Colonia Chuburná Hidalgo Inn, Mérida Yucatán.</p>
      <p><strong>Teléfono:</strong> <br> (999) 942 31 40 al 49</p>
      <p><strong>Correo:</strong> <br> matemati@www.uady.mx</p>
    </div>
    <div class="legal">
      <h2>Legal</h2>
      <p> <strong>@Todos los Derechos Reservados, FMAT 2018</strong> </p>
      <p> Esta página puede ser reproducida con fines no lucrativos, siempre y cuando no se mutile, se cite la fuente completa y su dirección electrónica, de otra forma requiere permiso previo por escrito de la institución. </p>
    </div>
    <div class="footer-buttons">
      <a href="#"><img src="../assets/fb.png" alt=""></a>
      <router-link to="/sitemap" class="sitemap-button"> <span @click="scrollMeToTop()">Mapa del <br> sitio</span></router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: 'fmat-footer',
  data () {
    return {

    }
  },
  methods: {
    scrollMeToTop () {
      window.scrollTo(0, 0)
    }
  }
}
</script>

<style lang="css" scoped>
  .footer{
    z-index: 2;
    display: grid;
    color: #F3F3F3;
    background: #082133;
  }

  .footer-buttons{
    margin-top: 54px;
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-column-gap: 30px;
    justify-items: center;
  }

  .sitemap-button{
    width: 98px;
    height: 52px;
    background: rgba(234, 198, 87, 0.712);
    border-radius: 4px;
    border-color: black;
    border-width: 1px;
    font-family: inherit;
    font-size: inherit;
    color: #000000;
    text-align: center;
    padding-top: 3px;
  }

  .contacto{
    width: 100%;
    text-align: justify;
}
  .legal{
    width: 100%;
    text-align: justify;
}

  @media only screen and (min-width: 150px) {
    .footer{
      height: 50%;
      padding: 8px 16px 25px 16px;
      grid-template-columns: 1fr;
      grid-template-rows: auto auto;
      grid-column-gap: 115px;
      position: inherit;
    }

    .legal{ display: none; }
  }

  @media only screen and (min-width: 640px) {
    .footer{
      padding: 8px 115px 25px 115px;
      grid-template-columns: repeat(2, 1fr);
      grid-column-gap: 115px;
      position: absolute;
    }

    .legal{ display: none; }
  }

  @media only screen and (min-width: 1000px) {
    .footer{
      padding: 8px 115px 25px 115px;
      grid-template-columns: repeat(3, 1fr);
      grid-column-gap: 115px;
      position: absolute;
    }

    .legal{ display: inherit; }
  }
</style>
