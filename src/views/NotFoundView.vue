<template>
    <div class="contenedor text-center">
        <h2 class="mt-4">No Encontrado</h2>
        <img src="@/assets/error.jpg" width="500px" height="500px">
        <h4>La página que buscas no existe. Favor de volver a Home.</h4>
        <v-btn @click="redireccionar" class="mt-3" elevation="5">Volver a Home</v-btn>
    </div>
</template>

<script>
export default {
    name: 'not-found-view',
    // props: {},
    data: function(){
        return {}
    },
    // computed: {},
    methods: {
        redireccionar() {
            this.$router.push('/');
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
    
</style>