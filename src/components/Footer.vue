<template>
    <div>
        <v-footer color="blue darken-4" padless>
            <v-row justify="center" no-gutters>
                <v-col col-12 class="pa-4 text-center white--text">
                    <strong>Bienvenido a vuetify</strong> {{ new Date().getFullYear() }} -
                </v-col>
            </v-row>
        </v-footer>
    </div>
</template>

<script>
export default {
    name: 'footer-comp',
    // props: {},
    data: function(){
        return {}
    },
    // computed: {},
    // methods: {}
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