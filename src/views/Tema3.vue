<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 3
      h1 Conflictos y problemas ambientales

    .row.justify-content-center.align-items-center.mb-5
      .row.justify-content-center.align-items-center
        .col-lg-5
        .col-lg-6
          p.aling-1.mb-0 Los conflictos ambientales se entienden como las desigualdades sociales, espaciales y temporales que se generan por el uso que hacen las personas, de los recursos y de los servicios ecosistémicos. Por su parte, un problema ambiental está relacionado con la deficiencia, afectación, exceso o pérdida de un recurso natural o de un servicio ambiental específico (Castro, 2018).
      .col-lg.order-1.order-lg-2
        .custom_box_left 
          p.mb-0 Para lograr identificar la oferta de servicios ambientales de la finca cafetera, también es necesario hacer un inventario que recoja tanto los conflictos como los problemas ambientales presentes en el territorio para, de esta manera, diseñar alternativas que permitan mitigar, corregir o prevenir situaciones que puedan afectar el desarrollo de la actividad productiva y su sostenibilidad. 
        p.aling-2.mt-2.text-color <b> Etter, 2002 </b> 
      .col-auto.mb-5.mb-lg-0.onTop.order-2.order-lg-1
        img(src="@/assets/curso/images/tema3/img_1.png" alt='AvatarTop', style="width:430px; display:block; margin:-6rem -3rem;").m-auto

    p.mb-3.text-center <b>Para diferenciar los conflictos de los problemas ambientales es importante tener en cuenta, ver tabla 1:</b>

    .titulo-sexto.color-acento-contenido
      p.mb-0 <b>Tabla 1 </b>

    .row.justify-content-center.align-items-center
      .col-lg-10
        .tabla-a.tabla
          table
            thead
              tbody
              tr
                td.text-center.text-white.th-3 #[strong Conflicto]
                td.text-center.text-white.th-3 #[strong Problema]            
              tr
                td.th-5 Enfrentamiento por hechos vinculados a la escasez, el deterioro o la privación de los recursos naturales. 
                td.th-5 E Se presentan de manera independiente de la escasez, deterioro o privación de los recursos naturales.  
                
              tr
                td.th-5 E Surgen como consecuencia de un problema ambiental. 
                td.th-5 E Surgen por situaciones relacionadas con afectaciones reales o potenciales de las condiciones del entorno. 
                
              tr
                td.th-5 E Pueden considerarse construcciones sociales y culturales susceptibles de cambio, según cómo se aborden y manejen.
                td.th-5 E Afectan la calidad del ambiente o de alguno de sus componentes. 
                
              tr
                td.th-5 E Es posible que vinculen problemas de datos, de intereses o de creencias.
                td.th-5 E Vinculan situaciones de carencia, deficiencia o exceso de un factor indeseado. 
              tr
                td.th-5 E Surgen en situaciones de desigualdad social y débil institucionalidad.
                td.th-5 E Su aparición no está condicionada por desigualdad social o débil institucionalidad. 

      p.mt-5.text-center <b> Estas son algunas generalidades de las problemáticas ambientales; se debe llevar registro de esto en una libreta personal de apuntes. </b>

      SlyderB(:datos="datosSlyder").fondo-11

    Separador 

    #t_3_1.titulo-segundo.p-4
      .h4 3.1 Origen de los conflictos ambientales

    p.mb-3 El surgimiento de los conflictos ambientales no es algo que suceda de la noche a la mañana, sino que, por el contrario, obedecen a una serie de situaciones que se van presentando de manera secuencial y paulatina hasta que llegan a etapas en las que se tornan inmanejables. Tales etapas están plenamente identificadas y es posible tomar acciones antes de que la situación se convierta en una crisis, que resulte perjudicial para las partes involucradas. 

    p.mb-3.text-center <b> Se presenta el listado de etapas que configuran un conflicto ambiental: </b>

      
    .row.justify-content-center.align-items.p-3
      .col-lg-8
        TabsA.color-primario.mb-5
    
          .tarjeta_tab.back-tab.p-4(titulo="1. Formación")
            
            .row 
              .col-lg-8.mb-4
                h4 1. Formación
                p.mb-3  Se reconoce la existencia del problema ambiental pero no se toman acciones al respecto. 
                
          .tarjeta_tab.back-tab.p-4(titulo="2. Resignificación de los procesos agrícolas")
            
            .row 
              .col-lg-8.mb-4
                h4 2. Surgimiento
                p.mb-3 Se definen los intereses y las posiciones de los actores involucrados. 

          
          .tarjeta_tab.back-tab.p-4(titulo="3. Escalamiento")
            
            .row 
              .col-lg-8.mb-4
                h4 3. Escalamiento
                p.mb-3 Cada parte desarrolla estrategias para la confrontación, se da un distanciamiento entre las partes. 
 


          .tarjeta_tab.back-tab.p-4(titulo="4. Crisis")
            
            .row 
              .col-lg-8.mb-4
                h4 4. Crisis

                p.mb-3 Se da una confrontación. no hay diálogo ni negociación y las partes buscan imponer sus voluntades e intereses. 

          .tarjeta_tab.back-tab.p-4(titulo="5. Desescalada")
            
            .row 
              .col-lg-8.mb-4
                h4 5. Desescalada
                p.mb-3 Se reduce la tensión y se establecen estrategias de diálogo, participación y cooperación
 


          .tarjeta_tab.back-tab.p-4(titulo="6. Maduración")
            
            .row 
              .col-lg-8.mb-4
                h4 6. Maduración

                p.mb-3 Proceso de búsqueda de acuerdos e interese que fomenten espacios de diálogo y discusión. 
          
          .tarjeta_tab.back-tab.p-4(titulo="7. Transformación")
            
            .row 
              .col-lg-8.mb-4
                h4 7. Transformación

                p.mb-3 Las partes encuentran salidas al conflicto. Hay trabajo colaborativo y constructivo. 

      .col-lg-4
        img(src="@/assets/curso/images/tema3/img_3.png", style="width: 300px").m-auto

    Separador 

    #t_3_2.titulo-segundo.p-4
      .h4 3.2 Acciones de mitigación de conflictos ambientales
    
    p.mb-3 La resolución de los conflictos ambientales abarca una amplia gama de alternativas, las cuales se pueden aplicar dependiendo de la naturaleza del conflicto, de las motivaciones de los actores involucrados y de las circunstancias que rodeen la situación, entre otros factores. 

    p.mb-3.text-center <b>Sobre las acciones de mitigación de conflictos en el orden ambiental, se puede conocer las generalidades y aspectos clave que, a continuación, se presentan:</b>
  .container.bg-white.p-4.p-md-5.fondo-video-1
    figure.p-5
      .video
        iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)

    p.mb-3.text-center <b> En cuanto a los mecanismos alternativos para la resolución de conflictos ambientales, se presenta algunas especificaciones que se debe tener presentes: </b>
  .container.bg-white.p-4.p-md-1.container-bottom 
    .row.justify-content-center.align-items.p-3
      .col-lg-4
        img(src="@/assets/curso/images/tema3/img_4.png", style="width: 300px").m-auto
      .col-lg-8
        TabsA.color-primario.mb-5
  
          .tarjeta_tab.back-tab.p-4(titulo="1. Negociación")
            
            .row 
              .col-lg-8.mb-4
                h4 1. Negociación
                p.mb-3  Las partes intercambian información para lograr una salida que satisgafa las necesidades de las dos partes. 
                
          .tarjeta_tab.back-tab.p-4(titulo="2. Diálogo")
            
            .row 
              .col-lg-8.mb-4
                h4 2. Diálogo
                p.mb-3 A través de este proceso las dos partes exponen sus razones y puntos de vista respecto a la situación para llegar a acuerdos. 
            
          
          .tarjeta_tab.back-tab.p-4(titulo="3. Facilitación")
            
            .row 
              .col-lg-8.mb-4
                h4 3. Facilitación

                p.mb-3 A través de la intervención de un tercero se produce la interacción entre las partes para cumplir objetivos previamente trazados. 


          .tarjeta_tab.back-tab.p-4(titulo="4. Mediación")
            
            .row 
              .col-lg-8.mb-4
                h4 4. Mediación
                p.mb-3 Una tercera parte neutral e imparcial asiste a las partes para que negocien. 


          .tarjeta_tab.back-tab.p-4(titulo="5. Horizontes del suelo")
            
            .row 
              .col-lg-8.mb-4
                h4 5. Resolución
                p.mb-3 Atiende los intereses y necesidades de las partes pero centrada en una disputa concreta




















</template>

<script>
export default {
  name: 'Tema3',
  data: () => ({
    datosSlyder: [
      {
        titulo: 'Realidad y deber ser',
        texto:
          'Las problemáticas ambientales se relacionan con las diferencias existentes entre lo que se tiene en la realidad y lo que se podría llegar a tener bajo unas condiciones ideales u óptimas.',
        imagen: require('@/assets/curso/images/tema3/img_2.png'),
      },
      {
        titulo: 'Relativa conexión entre problemas y conflictos',
        texto:
          'La afectación de los ecosistemas es una problemática ambiental pero no siempre está ligada a algún conflicto en particular.',
        imagen: require('@/assets/curso/images/tema3/img_5.png'),
      },
      {
        titulo: 'Problemáticas ambientales más comunes',
        texto:
          'Contaminación del agua, tráfico de especies silvestres, acumulación de residuos sólidos, contaminación del aire, deforestación e incendios forestales, degradación de suelos.',
        imagen: require('@/assets/curso/images/tema3/img_6.png'),
      },
      {
        titulo: 'Conflictos e inequidad',
        texto:
          'Por otro lado, los conflictos ambientales más comunes están relacionados con la inequidad en el acceso a los servicios ecosistémicos y la pérdida de capacidad para el acceso a la tierra..',
        imagen: require('@/assets/curso/images/tema2/img_7.png'),
      },
      {
        titulo: 'Principales conflictos ambientales',
        texto:
          'Estos son algunos ejemplos de conflictos presentes en diversos territorios.',
        imagen: require('@/assets/curso/images/tema3/img_8.svg'),
      },
    ],
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
