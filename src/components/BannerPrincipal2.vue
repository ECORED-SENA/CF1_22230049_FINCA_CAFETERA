<template lang="pug">
.banner-principal
  .container.tarjeta.position-relative(
    :style="{'background-image': globalData.fondoBannerPrincipal ? `url(${globalData.fondoBannerPrincipal})` : 'none'}"
  )
    .row.banner-principal__row.position-relative.justify-content-center.align-items-center
      .col-lg-7.col-xxl-6.py-4.py-sm-5.banner-principal__info.ps-5
        .banner-principal__componente
          h1.mb-0(v-html="globalData.componenteFormativo")
        .col-lg-12
          .banner-principal__descripcion
            p.mb-0(v-html="globalData.descripcionCurso")
        .banner-principal__accion
          router-link.boton(:to="{name: iniciarLnk.nombreRuta }")
            span.me-1 Iniciar
            i.fas.fa-angle-right

      .d-none.d-lg-block.col-lg-5.px-0.position-relative.img-p
        img(:src="globalData.imagenBannerPrincipal" style="width: 520px")
    .d-none.d-xl-block.imagen_flotante_5: img(src="@/assets/curso/images/header/banner-principal.png" alt='' , style="width:500px; display:block; margin:0 auto;")
    .imagen_flotante_1.d-none.d-xl-block: img(src="@/assets/curso/images/header/flotante_1.png" alt='' , style="width:100px; display:block; margin:0 auto;")
    .imagen_flotante_2.d-none.d-xl-block: img(src="@/assets/curso/images/header/flotante_2.png" alt='' , style="width:100px; display:block; margin:0 auto;")
    .d-none.d-xl-block.imagen_flotante_3: img(src="@/assets/curso/images/header/flotante_3.png" alt='' , style="width:100px; display:block; margin:0 auto;")
    .d-none.d-xl-block.imagen_flotante_4: img(src="@/assets/curso/images/header/flotante_4.png" alt='' , style="width:50px; display:block; margin:0 auto;")
    .d-none.d-xl-block.imagen_flotante_6: img(src="@/assets/curso/images/header/flotante_6.png" alt='' , style="width:50px; display:block; margin:0 auto;")
    .d-none.d-xl-block.imagen_flotante_7: img(src="@/assets/curso/images/header/flotante_5.png" alt='' , style="width:450px; display:block; margin:0 auto;")
  
  

</template>

<script>
import mixins from '../components/plantillaMixins'
export default {
  name: 'BannerPrincipal2',
  mixins: [mixins],
  computed: {
    globalData() {
      return this.$config.global
    },
  },
}
</script>

<style lang="sass">
.img-p
  top: 3%
  right: 1%
.fondo-contenido
  position: absolute
  padding: 0px
  z-index: 2
  height: 100%
  width: 100%
.banner-principal__info
  padding-left: 95px  !important
  margin-top: 5px
  z-index: 3
.banner-principal
  p, h1, h2, h3, h4, h5, h6
    color: $color-banner-text

  .tarjeta
    background-color: $color-banner-fondo
    background-size: cover
    background-position: center
    height: 32rem

  &__info
    display: flex
    flex-direction: column
    justify-content: center

  &__programa
    display: flex
    align-items: center
    margin-bottom: 20px

  &__componente
    margin-bottom: 20px
    h1
      line-height: 1.1em

      @media (max-width: $bp-max-xs)
        font-size: 2em

  &__descripcion
    margin-bottom: 20px

  &__row
    @if $banner-principal-img-x == 'derecha'
      justify-content: space-between
    @else
      justify-content: space-around
      .banner-principal__img
        padding-right: 1.5rem!important
      @media (min-width: $bp-min-sm)
        .banner-principal__img
          padding-right: 3rem!important

  &__img
    animation: scale 5s ease-in-out infinite alternate
    @if $banner-principal-img-y == 'arriba'
      align-self: flex-start
      padding-bottom: 1.5rem
      @media (min-width: $bp-min-sm)
        padding-bottom: 3rem!important
    @else if $banner-principal-img-y == 'abajo'
      align-self: flex-end
      padding-top: 1.5rem
      @media (min-width: $bp-min-sm)
        padding-top: 3rem!important
    @else
      align-self: center
      padding-top: 1.5rem
      padding-bottom: 1.5rem
      @media (min-width: $bp-min-sm)
        padding-top: 3rem!important
        padding-bottom: 3rem!important


.imagen_flotante
  &_1
    animation: float1 3.5s ease-in-out infinite alternate
    position: absolute
    width: 242px
    height: 200px
    top: 30%
    left: 54%
    z-index: 99
  &_2
    animation: float1 3.5s ease-in-out infinite alternate
    position: absolute
    width: 223px
    height: 168px
    bottom: 45%
    right: 20%
    z-index: 99
  &_3
    animation: float1 3.5s ease-in-out infinite alternate
    position: absolute
    width: 90rem
    bottom: 17%
    left: 25%
    z-index: 99
  &_4
    animation: float1 4s ease-in-out infinite alternate
    position: absolute
    width: 350px
    height: 294px
    top: 38%
    left: 75%
    z-index: 99
  &_5
    position: absolute
    width: 480px
    top: 25%
    left: 60%
    z-index: 99
  &_6
    filter: blur(2px)
    animation: float1 2.7s ease-in-out infinite alternate
    position: absolute
    width: 267px
    top: 30%
    right: 3%
    z-index: 99
  &_7
    animation: float1 2.5s ease-in-out infinite alternate
    position: absolute
    width: 180px
    bottom: 20%
    right: 15%
    z-index: 99
  &_8
    filter: blur(1px)

    animation: float1 3s ease-in-out infinite alternate
    position: absolute
    width: 50px
    bottom: 20%
    right: 8%
    z-index: 99

@keyframes float1
  0%
    transform: translateY(20px)

  100%
    transform: translateY(0px)
@keyframes scale
  0%
    transform: scale(1.1)

  100%
    transform: scale(1)


@media (max-width: $bp-max-md)
  .fondo-contenido
    display: none
  .fondo-contenido2
    background-repeat: no-repeat
    background-size: cover
</style>
