<template>
    <div class="productos">
        <div v-for="mueble in muebles" :key="mueble.id" class="cajas">
            <img :src="mueble.foto" :alt="mueble.nombre">
            <div class="contenedor">
                <h3>{{ mueble.nombre }}</h3>
                <div class="cont_inf">
                    <p>{{ mueble.prec }}</p>
                    <router-link :to="'/detalles/' + mueble.id" class="links">Ver Detalles</router-link>
                </div>
                
            </div>
            
        </div>
        
    </div>
</template>

<script>
import { muebles } from '@/listprod'


export default {
    data(){
        return{
            mueble: {},
            muebles: muebles
        }

    }
}
</script>

<style lang="sass" scoped>
.productos

    display: flex
    flex-direction: row
    justify-content: center
    align-items: center
    height: 100%

    
    .cajas
        margin: auto
        height: 400px
        width: 350px
        border-radius: 20px
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1)

        img
            border-radius: 20px 20px 0 0
            height: 250px
            width: 350px

        .contenedor
            margin: 20px

            .cont_inf
                margin-top: 30px
                display: flex
                flex-direction: row
                justify-content: space-between

                p
                    color: #B519B8
                    font-weight: bold

                .links
                    list-style: none
                    text-decoration: none
                    background-color: #14C9E1
                    color: white
                    border: none
                    padding: 5px
                    border-radius: 20px
        
        

</style>