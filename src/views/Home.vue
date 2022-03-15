<template>
    <div class="home">
        <img alt="Vue Logo" src="../assets/logo.png">
        <HelloWorld msg="Welcome to your new app" />
    </div>
</template>

<script>
import HelloWorld from '@/components/HelloWorld';
export default {
    name: 'Home',
    components: {
        HelloWorld
    }
}
</script>