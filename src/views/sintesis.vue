<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    .titulo-cafe.mb-5
      h3.mb-0.text-center.color-secundario.font-weight-bold.me-5
        |Síntesis
      .titulo-cafe_icon: img(src='@/assets/curso/17.svg' alt='Icono de la categoria')
    
    p.aling-1.mb-3 Se ha finalizado el estudio de los contenidos de este componente formativo. En este punto, se invita a hacer un análisis de la estructura que se muestra a continuación. Se debe registrar una síntesis propia en una libreta de apuntes personal. Se debe repasar los puntos que se considere necesario. ¡Adelante!


      .row.justify-content-center.align-items.mb-3
        .col-lg-11
          img(src="@/assets/curso/images/tema4/sintesis.svg", alt= "") 

    

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
