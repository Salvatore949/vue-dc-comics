<template>
    <footer>
        <div id="jumbo" :src="'link'" :style="{'background-image': 'url(' + require('@/assets/img/footer-bg.jpg') + ')'}"></div>
    </footer>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style>
 #jumbo{
     min-height: 65vh;
     width: 100%;
 }

</style>