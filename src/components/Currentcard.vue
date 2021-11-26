<template>
    <section id="product_card">
        <img id="product_image" :src="details.thumb">
        <p>{{details.series}}</p>
    </section>
</template>

<script>

export default {
    name: 'Currentcard',
    props:{
        details:Object
    }

}
</script>

<style>
#product_card{
    padding:30px 15px;
    color: white;
}

</style>