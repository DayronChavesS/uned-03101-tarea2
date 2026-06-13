<template>
<p>UNIVERSIDAD ESTATAL A DISTANCIA</p>
<p>ESCUELA CIENCIAS EXACTAS Y NATURALES</p>
<p>PROGRAMA DE INFORMÁTICA</p>
<p>CÁTEDRA DE DESARROLLO DE SOFTWARE</p>

<p>Tarea No.2</p>
<p>Contenedores</p>

<p>Nombre del Curso:  Programación Web Avanzada</p>
<p>Grupo No. 1</p>
<p>Nombre del Tutor: Norberth Brunner Agüero</p>

<p>Nombre Completo: Chaves Sandoval Dayron Antony</p>
<p>Número de cédula: 3-524-018</p>

<p>Centro Universitario de Turrialba</p>
<p>24 de Junio</p>
<p>II CUATRIMESTRE 2024</p>
</template>

<script>
export default { name: 'App',} 
</script>


<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
