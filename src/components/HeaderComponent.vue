<template>
    <div class="mt-nav">
        <div class="container">
            <nav class="d-flex justify-content-between align-items-center">
                <img src="/public/logo.png" alt="logo" id="mt-logo">
                <ul class="list-unstyled d-flex">
                    <li class="mt-3 me-2"><a class="mt-delete" href="">Accedi</a></li>
                    <li class="mt-3"><a class="mt-delete" href="">Registrati</a></li>
                </ul>
            </nav>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'HeaderComponent',
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;

    .mt-nav{
        background-color: $teal-color;
        #mt-logo{
            width: 200px;
        }
        .mt-delete{
            color: $white-color;
            text-decoration: none;
            border: 1px solid $white-color;
            padding: 6px 12px;
            border-radius: 12px;

            &:hover{
                background-color: $white-color;
                color: $teal-color;
                transition: 0.3s;
            }
        }
    }

</style>