<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    p.mb-5 El siguiente mapa conceptual integra los criterios y especificidades de los conocimientos expuestos en el presente componente formativo.

    .row.justify-content-center
      .col-lg-10.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis.svg", alt="A continuación, se presenta la síntesis del componente formativo: Generalidades de la gestión del talento humano donde se presenta la identificación de las necesidades del talento humano, la cual se compone del análisis de necesidades, instrumentos de recolección de información, descripción de cargos, perfil laboral, funciones, reclutamiento y selección, y contratación, por otro lado se encuentra la estructura organizacional y esta se compone por los modelos de estructuras organizacionales, como lo son las planas, horizontales, internacionales, modulares y virtual. Por último se encuentra gestión del talento humano, agrupado con las fases o procesos, acciones, características, objetivos y marco legal.")
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
