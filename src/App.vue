<template>
  <div>
    <div id="logo_tit">
      <h1>4TUKEA</h1>
    </div>
    <div id="cuerpo">
      <nav id="menu">
        <router-link to="/" class="links">Inicio</router-link>
        <router-link to="/productos" class="links">Productos</router-link>
        <router-link to="/contacto" class="links">Contacto</router-link>
      </nav>
      <div id="vista">
        <router-view/>
      </div>
      <div id="pie">
        <p class="itempie">Políticas de privacidad</p>
        <i class="fa-brands fa-instagram itempie"></i>
        <p class="itempie">Términos y condiciones</p>
      </div>
    </div>
    
  </div>
</template>

<style lang="sass">
*
  padding: 0
  margin: 0

  #logo_tit
    text-align: center
    font-size: 28px
    font-family: 'Inknut Antiqua', serif

  #cuerpo
    display: flex
    flex-direction: column

    #menu
      display: flex
      justify-content: center
      align-items: center
      background: #EDEDED
      font-size: 20px
      height: 8vh
      
      
      .links
        color: black
        list-style: none
        text-decoration: none
        padding-inline: 30px
        font-weight: bold

    #vista
      height: 69vh

        
    #pie
      height: 8vh
      background: #EDEDED
      display: flex
      flex-direction: row

      .itempie
        margin: auto
      
      i
        font-size: 20px


</style>
