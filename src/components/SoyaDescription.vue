<template>
    <div class="container description">
        <blockquote class="blockquote text-center">
            <h3 class="mb-1 font-italic green-text font-weight-bold">
                To take on a language is to take on a world, a culture.
            </h3>
            <footer class="blockquote-footer"><cite title="Franz Fanon">Franz Fanon</cite></footer>
        </blockquote>

        <div class="row my-5 justify-content-center">
            <div class="col-7 mt-5">
                <img class="img-fluid w-50" src="../assets/soyalogo.png" />
                <p class="green-text font-weight-bold display-5">Soya Beans<br>Japanese Language School</p>
                <p class="smaller"> is very willing to help you especially with your dream of traveling, studying or working in Japan.</p>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>

    @media (max-width: 576px) {
        h3{
            font-size: 1.3rem;
        }
        span {
            font-size: 1.3rem !important;
        }
    }
    .description {
      margin-top: 1em;
      z-index: 10;
    }
    .smaller {
        font-size: 1.2rem;
    }
    .display-5{
        font-size: 2.4em;
    }
</style>