<template>
    <div class="Home">
        <p>Welcome to the Home Page!</p>
        <base-button :disabled="false" color="primary">Test button</base-button>
        <base-button :disabled="false" color="warn">Test button</base-button>
        <base-button :disabled="false" color="danger">Test button</base-button>
    </div>
</template>

<script>
import BaseButton from '../components/base_button.vue';

export default {
    name: 'HomePage',
    components: {
        BaseButton,
    },

}
</script>

<style scoped>
.Home {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    text-align: center;
    margin-top: 60px;
}
</style>
