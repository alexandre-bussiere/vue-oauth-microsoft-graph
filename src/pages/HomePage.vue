<template>
    <div class="Home">
        <async-component @click="Wait"/>
    </div>
</template>

<script>
import AsyncComponent from '../components/AsyncComponent.vue';
export default {
    name: 'HomePage',
    components: {
        AsyncComponent,
    },
    methods: {
        Wait() {
            return new Promise((resolve) => {
                setTimeout(() => {
                console.log('Operation complete!');
                resolve();
                }, 2000); 
            });
        }
    }
}

</script>

<style scoped>
.Home {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    text-align: center;
    margin-top: 60px;
}
</style>
