<template>
  <div class="detalles">
    <div id="caja">
        <img :src="mueble.foto">
        <div id="cajatexto">
            <h1>{{ mueble.nombre }}</h1>
            <p id="descripcion">{{ mueble.desc }}</p>
            <div id="cajita">
                <p id="cos">{{ mueble.prec }}</p>
                <router-link to="/productos" class="links" id="cos">Comprar</router-link>
            </div>
        </div>
        
      

    </div>
  </div>
</template>

<script>
import { muebles } from '@/listprod'

export default {
  data() {
    return {
      mueble: {}
    };
  },
  created() {
    const muebleId = this.$route.params.id;
    this.mueble = muebles.find(m => m.id == parseInt(muebleId));
  }
}
</script>

<style lang="sass" scoped>
.detalles
    display: flex
    flex-direction: row
    justify-content: center
    align-items: center
    height: 100%

    #caja
        display: flex
        flex-direction: row
        margin: auto
        

        img
            width: 600px
            height: 300px
            margin: 20px
            border-radius: 10px

        #cajatexto
            width: 600px
            height: 300px
            margin: 20px

            #descripcion
                margin-top: 30px
                font-size: 18px

                
            #cajita
                display: flex
                flex: row
                justify-content: space-between
                margin-top: 30px

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