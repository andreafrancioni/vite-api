<script>
export default {
    name: "AppCard",
    props: ["shop"],
}
</script>

<!-- Genera una card mostrando i dati passati dal props chiamato shop -->
<template>
    <div class="wrapper">
        <div class="card">
            <img src="https://creazilla-store.fra1.digitaloceanspaces.com/cliparts/3152059/beer-clipart-md.png" alt="">
            <h3>{{ shop.name }}</h3>
            <p>{{ shop.city }}</p>
            <p>{{ shop.street }}</p>
            <p>{{ shop.phone }}</p>
            <p>{{ shop.brewery_type }}</p>
            <p>{{ shop.website_url }}</p>


        </div>
    </div>
</template>

<style scoped>
.wrapper {
    padding: 1rem;
    width: 20rem;
}

.card {
    padding: 1rem;
    background: gold;
    border: 2px solid white;
    color: black
}

img {
    width: 3rem;
}
</style>