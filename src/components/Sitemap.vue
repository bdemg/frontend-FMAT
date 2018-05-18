<template lang="html">
  <div class="">
    <fmat-header></fmat-header>
      <div class="body">
        <div class="sidebar"></div>
        <div class="content">
          <h1 class="page-header"> <strong>Mapa del sitio</strong> </h1>

          <div class="map">
            <ul>
              <li class="nav-header"><strong>FMAT</strong></li>
              <li ><router-link to="/historia">¿Quienes somos?</router-link></li>
              <li ><router-link to="/organizacion">Organización</router-link></li>
              <li ><router-link to="/directorio">Directorio</router-link></li>
              <li ><router-link to="/academicos">Académicos</router-link></li>
            </ul>

            <ul>
              <li class="nav-header"><strong>Correo</strong></li>
              <li ><a href="https://login.microsoftonline.com/" >Office 365</a></li>
              <li ><a href="http://www.matematicas.uady.mx//listas-de-correo" >Listas de correo</a></li>
            </ul>

            <ul>
              <li class="nav-header"><strong>Planes de estudio</strong></li>
              <li ><a href="http://www.matematicas.uady.mx//licenciaturas" >Licenciaturas</a></li>
              <li ><a href="http://www.matematicas.uady.mx//especializacion" >Especialización</a></li>
              <li ><a href="http://www.matematicas.uady.mx//maestrias" >Maestrías</a></li>
            </ul>

            <ul>
              <li class="nav-header"><strong>Calendario Escolar</strong></li>
              <li ><a href="http://www.matematicas.uady.mx//files/calendarios/escolar/2018/Calendario-ene-jul-2018-MEyA.pdf" >Escolar (MEyA)</a></li>
              <li ><a href="http://www.matematicas.uady.mx//files/calendarios/escolar/2018/Calendario-ene-julio-2018-MEFI.pdf" >Escolar (MEFI)</a></li>
              <li ><a href="http://www.matematicas.uady.mx/files/calendarios/extraordinarios/2017/CalendarioExtraordinarios-AGO-DIC-2017-fechas-asignaturas.pdf" >Extraordinarios</a></li>
              <li ><a href="http://www.matematicas.uady.mx//calendario-escolar/historicos" >Históricos</a></li>
            </ul>

            <ul>
              <li class="nav-header"><strong>Sitios</strong></li>
              <li ><a href="http://intranet.matematicas.uady.mx/portalweb/index.php/procma-inicio" >Programa de Cuidado del Medio Ambiente</a></li>
              <li ><a href="http://intranet.matematicas.uady.mx/sgc/" >Sistema de Gestión de Calidad</a></li>
              <li ><a href="https://intranet.matematicas.uady.mx/personal/enrique.ayala/web/cisco/" >Academia de Redes Cisco FMAT - UADY</a></li>
            </ul>

            <ul>
              <li class="nav-header"><strong>Servicios</strong></li>
              <li ><a href="https://intranet.matematicas.uady.mx/enlinea/" >EnLínea (Dokeos)</a></li>
              <li ><a href="https://intranet.matematicas.uady.mx/enlinea2/" >EnLínea2 (Moodle)</a></li>
              <li ><a href="http://es.uadyvirtual.uady.mx/" >UADY Virtual</a></li>
              <li ><a href="https://intranet.matematicas.uady.mx/personal/" >Carpetas de Profesores</a></li>
              <li ><a href="https://intranet.matematicas.uady.mx/servicios/salas/" >Reservación de Salas</a></li>
              <li ><a href="http://www.matematicas.uady.mx//servicios/centro-de-asesoria-en-matematicas" >Centro de Asesoría en Matemáticas</a></li>
            </ul>

            <ul>
              <li class="nav-header"><strong>Departamentos</strong></li>
              <li ><a href="http://www.matematicas.uady.mx//servicios/ctic" >CTIC-FMAT</a></li>
              <li ><a href="http://www.matematicas.uady.mx//servicios/lmec" >Laboratorio de Mantenimiento</a></li>
              <li ><a href="https://intranet.matematicas.uady.mx/portal/dme/" >Matemática Educativa</a></li>
            </ul>

            <ul>
              <li class="nav-header"><strong>Unidad de Extensión</strong></li>
              <li><a href="https://intranet.matematicas.uady.mx/ue/educonm/" >EduconM (Moodle)</a></li>
              <li><a href="http://www.bolsadetrabajo.uady.mx/" >Bolsa de Trabajo</a></li>
              <li><a href="http://www.matematicas.uady.mx//diplomados" >Diplomados</a></li>
            </ul>

            <ul>
              <li class="nav-header"><strong>Cuerpos Académicos</strong></li>
              <li><a href="https://intranet.matematicas.uady.mx/portalweb/index.php/ca-terco" >Tecnologías Emergentes en Computación</a></li>
              <li><a href="http://www.clir-lab.org" >Modelado y Simulación Computacional de Sistemas Inteligentes</a></li>
            </ul>

            <ul>
              <li class="nav-header"><strong>Eventos</strong></li>
              <li><a href="https://intranet.matematicas.uady.mx/cams/" >Concurso Anual de Matemáticas del Sureste</a></li>
              <li><a href="http://intranet.matematicas.uady.mx/portalweb/index.php/omm-inicio" >Olimpiada Mexicana de Matemáticas</a></li>
            </ul>
          </div>

        </div>
        <div class="sidebar"></div>
      </div>
    <fmat-footer></fmat-footer>
  </div>
</template>

<script>
import FmatHeader from '@/components/FmatHeader'
import FmatFooter from '@/components/FmatFooter'

export default {
  name: 'sitemap',
  components: {
    FmatHeader, FmatFooter
  },
  data () {
    return {

    }
  }
}
</script>

<style lang="css" scoped>
  .map{
    display: grid;
    grid-column-gap: 42px;
    grid-row-gap: 24px;
    justify-items: stretch;
    text-align: center;
  }

  .map ul{
    padding-left: 0px;
  }

  .map li{
    list-style-type: none;
    border-bottom: 1px solid #DDD;
    padding: 8px 0 8px 0;
  }

  ul li:first-child{
    padding-bottom: 16px;
  }

  .nav-header{
    font-size: 18px;
  }

  @media only screen and (min-width: 150px) {
      .map{
        grid-template-columns: 1fr;
      }
  }

  @media only screen and (min-width: 640px) {
    .map{
      grid-template-columns: repeat(2, 1fr);
    }
  }

</style>
