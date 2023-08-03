<template>
  <div class="principal-container">
    <v-container >
      <v-row justify="center" class="mt-16" >
        <v-col cols="12" sm="8" class="principal-box">
            <div>
                <h1>Desafía las expectativas de los MOBA</h1>
                <p>Épicos héroes y acción sin cesar en múltiples campos de batalla</p>
                <div class="text-center">
                  <v-btn @click="redireccionar" color="orange darken-2" dark>Ver héroes</v-btn>
                </div>
            </div>
        </v-col>
      </v-row>
    </v-container>

    <v-alert border="left" color="purple darken-1" dark class="py-5 mt-14" style="opacity: 0.8">      
      ¡Te damos la bienvenida al Nexo! ¡En este reino entre reinos, todo es posible! Elige entre decenas de héroes legendarios de 
      todo el panteón de Blizzard, personaliza sus talentos y habilidades en medio del combate y lucha en una infinidad de campos 
      de batalla que redefinen el género. ¡Esto no es un MOBA promedio, eso es Heroes of th Storm!      
    </v-alert>
  </div>
</template>

<script>

  export default {
    name: 'Home-view',
    // props: {},
    data: function(){
      return {}
    },
    // computed: {},
    methods: {
      redireccionar() {
        this.$router.push('/heroes');
      }
    },
    // watch: {},
    // components: {},
    // mixins: [],
    // filters: {},
    // -- Lifecycle Methods
    // -- End Lifecycle Methods
  }
</script>

<style scoped>
  .principal-container {
    height: 100%;
    background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('@/assets/fondo1.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
  }
  .principal-box {
    border: 1px solid white;
    color: white;
  }
</style>