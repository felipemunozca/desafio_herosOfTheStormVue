<template>
    <div>
        <v-app-bar color="blue darken-4" dark dense>
            <div class="d-flex justify-center flex-grow-1" >
                <v-btn @click="redireccionar" color="blue darken-3" >
                    <v-icon>mdi-home</v-icon>
                    Home
                </v-btn>
            </div>
        </v-app-bar>
    </div>
</template>

<script>
export default {
    name: 'navbar-comp',
    // props: {},
    data: function(){
        return {}
    },
    // computed: {},
    methods: {
        redireccionar() {
            if (this.$route.path == '/') {
                alert('Ya se encuentra en la vista Home');
                return;
            }
            this.$router.push('/');
            
            // ambos códigos hacen lo mismo.
            // if (this.$route.path == '/') {
            //     alert('Ya se encuentra en la vista Home');
            // } else {
            //     this.$router.push('/');
            // }
        },
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