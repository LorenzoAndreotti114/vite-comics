<script>
    import HeaderApp from './components/HeaderApp.vue';
    import MainApp from './components/MainApp.vue';
    import AppFooter from './components/AppFooter.vue';

    export default {
        components: {
            HeaderApp,
            MainApp,
            AppFooter,
        },
        
        data() {
            return {

            }
        }
    }

</script>

<template>

    <HeaderApp />

    <MainApp />

    <AppFooter />
  
</template>

<style scoped>

</style>
