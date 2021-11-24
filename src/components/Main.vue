<template>
<main>
    <div id="container">
        <ul id="topics">
            <li v-for="selection, i of chooseItem" :key="i">{{selection.paragraph}}</li>
        </ul>
    </div>
</main>
</template>

<script>
export default {
    nam: 'Main',
        name: 'Navbar',
    data: () => ({
        chooseItem : [
            {
                "img":"buy-comics-shop-locator.png",
                "paragraph":"DIGITAL COMICS"
            },
            {
                "img":"buy-comics-merchandise.png",
                "paragraph":"DC MERCHANDISE"
            },
            {
                "img":"buy-comics-shop-locator.png",
                "paragraph":"SUBSCRIPTION"
            },
            {
                "img":"buy-comics-subscriptions.png",
                "paragraph":"COMIC SHOP LOCATOR"
            },
            {
                "img":"buy-dc-power-visa.svg",
                "paragraph":"DC POWER VISA"
            }

        ]
    }

)}

</script>

<style>

#container{
   background-color:rgb(29, 102, 131) ; 
}

#topics{
    width: 60%;
    margin: 0 auto;
    color: #ffffff;
    
}
#topics > li{
    padding: 20px;
}

</style>