<template>
    <h3>Columnas</h3>
    <router-link to="/columns">Columnas</router-link> 


</template>

<script>
    import axios from 'axios'
    export default{
        name:'ColumnsList',
        data(){
            return{
                columns:null
            }
        },
        methods:{
            list(){
                axios.get('')
                     .then(res => this.directors = res.data.obj);
            }
        },
        mounted(){
            this.list()
        }
    };
</script>

<style scoped>

</style>