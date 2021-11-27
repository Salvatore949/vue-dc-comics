<template>
<main>
    <div id="container">
        <ul id="topics">
            <li v-for="selection, i in chooseItem" :key="i">
                <img id="itemsNav" :src=" require('@/assets/img/' + selection.img)">
                <p id=paragraph_selected>{{selection.paragraph}}</p>
            </li>
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

#topics{
    display: flex;
    align-items: center;
    list-style-type: none;
    font-size: 15px;
}

#topics > li{
    padding: 20px;
    display: flex;
}

#itemsNav{
 margin-right:10px;
 width: 60px;
}

#paragraph_selected{
    font-size:10px;
    display: flex;
    align-items: center;

}

</style>