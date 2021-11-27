<template>
    <footer>
    <div id="below_text" :src="'link'" :style="{'background-image': 'url(' + require('@/assets/img/footer-bg.jpg') + ')'}">

        <div id="footer_text">
            <ul id="texts">
                <li v-for="paragraphs, i in list_options" :key="i">
                  <b v-if="i === 0">{{paragraphs.text}}</b>
                  <p v-else>{{paragraphs.text}}</p>  
                </li>
            </ul>
            <ul id="texts_first">
                <li v-for="paragraphs_1, i in shop" :key="i">
                 <b v-if="i === 0">{{paragraphs_1.text}}</b>
                 <p v-else>{{paragraphs_1.text}}</p> 
                </li>
            </ul>
        </div>  
        <ul id="texts_second">
            <li v-for="paragraphs_2, i in DC_list" :key="i">
              <b v-if="i===0">{{paragraphs_2.text}}</b>
              <p v-else>{{paragraphs_2.text}}</p>
            </li>
        </ul>
        <ul id="texts_third">
            <li v-for="paragraphs_3, i in Sites_list" :key="i">
              <b v-if="i === 0">{{paragraphs_3.text}}</b>
              <p v-else>{{paragraphs_3.text}}</p>
              </li>
        </ul>
    </div>
    <div id="social">
      <button> SIGN UP NOW </button>
      <div>
        <img id="logos" v-for=" link, i in social_networks" :key="i" :src=" require('@/assets/img/' + link.logo )" >
      </div>
    </div>  
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
              "text": "SHOP"
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
            
        ],
        social_networks:[
          {
            "logo":"footer-facebook.png"
          },
          {
            "logo":"footer-periscope.png"
          },
          {
            "logo":"footer-pinterest.png"
          },
          {
            "logo":"footer-twitter.png"
          },
          {
            "logo":"footer-twitter.png"
          }
        ],
    })
}
</script>

<style>

  ul {
    list-style-type: none;
    color: white;
    }

  #below_text{
    display: flex;  
    padding-top:30px;
    padding-left:150px;
    line-height: 20px;
    min-height: 40vh;
  }

  #social{
    height:10vh;
    background-color: #303030;
    display: flex;
    justify-content: space-around;
  }

  #social > button{
    height:30%;
    margin:auto 0;
    border-radius: 0px;
    border:3px solid #204c76;
    background-color:transparent;
    color: #ffffff;
    padding: 10px;
    padding-bottom: 30px;
 
  }

  #social{
    height: 12vh;
  }

  #logos {
    margin-top: 25px;
    padding-left: 15px;
  }

</style>