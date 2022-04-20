<template>
    <footer>
        <p>Copyright &copy; 2021</p>
        <router-link to="/about" class="footer__link">About</router-link>
    </footer>
</template>

<style scoped>
a{
    color: #333;
}

footer{
    margin-top: 20px;
    text-align: center;
}

.footer__link{
    text-decoration: none;
    font-size: 1.5rem;
}
</style>

<script>
    export default {
        name: 'Footer',
    }

</script>
