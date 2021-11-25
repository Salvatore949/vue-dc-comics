<template>
    <footer>
        <ul id="texts">
            <li v-for="paragraphs, i in list_options" :key="i">{{paragraphs.text}}</li>
        </ul>
        <ul id="texts_first">
            <li v-for="paragraphs_1, i in shop" :key="i">{{paragraphs_1.text}}</li>
        </ul>
        <ul id="texts_second">
            <li v-for="paragraphs_2, i in DC_list" :key="i">{{paragraphs_2.text}}</li>
        </ul>
        <ul id="texts_third">
            <li v-for="paragraphs_3, i in Sites_list" :key="i">{{paragraphs_3.text}}</li>
        </ul>
        <div id="jumbo" :src="'link'" :style="{'background-image': 'url(' + require('@/assets/img/footer-bg.jpg') + ')'}"></div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    data: () => ({
        list_options : [
            {
              "text": "DC COMICS"
            },
            {
              "text": "Characters"
            },
            {
              "text": "Comics"
            },
            {
              "text": "Movies"
            },
            {
              "text": "TV"
            },
            {
              "text": "Games"
            },
            {
              "text": "Videos"
            },
            {
              "text": "News"
            }
        ],
        shop : [
            {
              "text": "Shop DC"
            },
            {
              "text": "Shop DC Collectibles"
            }
        ],
        DC_list: [
            {
              "text": "DC COMICS"
            },
            {
              "text": "Characters"
            },
            {
              "text": "Comics"
            },
            {
              "text": "Movies"
            },
            {
              "text": "TV"
            },
            {
              "text": "Games"
            },
            {
              "text": "Videos"
            },
            {
              "text": "News"
            }
            
        ],
        Sites_list : [
            {
              "text": "DC COMICS"
            },
            {
              "text": "Characters"
            },
            {
              "text": "Comics"
            },
            {
              "text": "Movies"
            },
            {
              "text": "TV"
            },
            {
              "text": "Games"
            },
            {
              "text": "Videos"
            },
            {
              "text": "News"
            }
            
        ]
    })
}
</script>

<style>
 #jumbo{
     min-height: 65vh;
     width: 100%;
}

ul {
    list-style-type: none;
}

</style>