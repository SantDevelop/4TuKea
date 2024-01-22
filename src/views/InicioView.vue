<template>
    <div class="inicio">
        <img src="https://cdn-icons-png.flaticon.com/512/3144/3144456.png" alt="" class="ini">
        <p class="ini">Es un hecho establecido hace demasiado tiempo que un lector se distraerá con el contenido del texto  de un sitio mientras que mira su diseño. El punto de usar Lorem Ipsum es que tiene una distribución  más o menos normal de las letras, al contrario de usar textos como por ejemplo "Contenido aquí, contenido aquí".</p>
        <router-link to="/productos" class="links ini">Ver Productos</router-link>
    </div>
</template>

<script>


export default {
    name: 'InicioView',
    components: {

    }
}
</script>

<style lang="sass" scoped>
.inicio
    display: flex
    flex-direction: column
    align-items: center
    justify-content: center
    text-align: center

    img
        width: 300px
        margin-top: 50px 

    p
        width: 700px
        margin-top: 50px
    .links
        list-style: none
        text-decoration: none
        padding-inline: 30px
        font-weight: bold
        background-color: #14C9E1
        color: white
        border: none
        padding: 5px
        border-radius: 20px
        margin-top: 50px



</style>