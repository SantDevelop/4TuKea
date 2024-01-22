<template>
    <div class="contacto">
        <div id="caja">
            <div id="cajaimagen" class="cajas">
                <img src="https://www.tribunacontactcenter.com/img/8838/8838_0772168001661370471.png">
            </div>
            
            <div id="formulario" class="cajas">
                <h1>CONTACTA CON NOSOTROS</h1>
                <div id="nomape">
                    <input type="text" class="entradas" placeholder="Nombre">
                    <input type="text" class="entradas" placeholder="Apellidos">
                </div>
                <input type="text" class="entradas" placeholder="Correo Electrónico">
                <textarea name="" id="" cols="30" rows="10" class="entradas" placeholder="¿En que podemos ayudarte?"></textarea>
                <div id="envio">
                    <router-link to="/" class="links" id="cos">Enviar</router-link>
                </div>
            </div>
        </div>
        
    </div>
</template>

<script>


export default {
    name: 'ContactoView',
    components: {

    }
}
</script>

<style lang="sass" scoped>
.contacto

    display: flex
    flex-direction: row
    justify-content: center
    align-items: center
    height: 100%

    #caja
        display: flex
        flex-direction: row
        justify-content: center

        margin: auto
        
        .cajas
            width: 600px

            img
                width: 500px
                margin: 20px
                border-radius: 10px

        #formulario
            text-align: center
            display: flex
            flex-direction: column
            width: 500px

            #nomape
                display: flex
                flex-direction: row
                justify-content: space-between

            .entradas
                background: #F8F8F8
                padding: 8px
                border-radius: 10px
                margin: 15px
                border: 0.5px solid grey
                box-shadow: 8px 4px 8px rgba(0, 0, 0, 0.2)

            #envio
                text-align: right
                margin-right: 15px
                .links
                    list-style: none
                    text-decoration: none
                    background-color: #14C9E1
                    color: white
                    border: none
                    padding: 5px
                    border-radius: 20px
                    padding-inline: 40px
                



</style>