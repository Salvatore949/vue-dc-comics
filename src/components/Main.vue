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
    name: 'Main',
    data: () => ({
        chooseItem : [
            {
                "img":"buy-comics-digital-comics.png",
                "paragraph":"DIGITAL COMICS"
            },
            {
                "img":"buy-comics-shop-locator.png",
                "paragraph":"DC MERCHANDISE"
            },
            {
                "img":"buy-comics-merchandise.png",
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

#topics{
    display: flex;
    align-items: center;
    list-style-type: none;
    font-size: 15px;
}

#topics > li{
    padding: 20px;
}

</style>