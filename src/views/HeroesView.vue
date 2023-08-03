<template>
    <div class="heroes-container">
        <v-container class="">
            <div>
                <h2 class="heroes-title my-4">Heroes</h2>
                <div class="heroes-icons mb-5">
                    <v-icon class="icon">mdi-sword</v-icon>
                    <v-icon class="icon">mdi-shield</v-icon>
                    <v-icon class="icon">mdi-crosshairs</v-icon>
                    <v-icon class="icon">mdi-heart-plus</v-icon>
                    <v-icon class="icon">mdi-dna</v-icon>
                </div>
            </div>

            <v-row justify="center mb-6">
                <v-col cols="12" sm="12">
                    <v-simple-table dark class="tabla">
                        <template v-slot:default>
                            <thead>
                                <tr>
                                    <th class="text-left">Héroes</th>
                                    <th class="text-left">Nombre</th>
                                    <th class="text-left">Función</th>
                                    <th class="text-left">Título</th>
                                    <th class="text-left">Ataque</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr v-for="(heroe, index) in heroes" :key="index">
                                    <td>
                                        <img :src="heroe.imagen" width="150px" height="150px"/>
                                    </td>
                                    <td>{{ heroe.nombre }}</td>
                                    <td>{{ heroe.funcion }}</td>
                                    <td>{{ heroe.titulo }}</td>
                                    <td>{{ heroe.ataque }}</td>
                                </tr>
                            </tbody>
                        </template>
                    </v-simple-table>
                </v-col>
            </v-row>
    </v-container>
    </div>
    
</template>

<script>
import { mapState } from 'vuex';

export default {
    name: 'heroes-view',
    // props: {},
    data: function(){
        return {}
    },
    computed: {
        ...mapState(['heroes']),
    },
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
    .heroes-container {
        height: 100%;
        background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('@/assets/fondo2.jpg');
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
    }
    .heroes-title {
        color: white;
        margin-top: 20px;
    }
    .heroes-icons .icon {
        color: lightgray;
        padding: 0 5px;
        font-size: 25px;
    }
</style>