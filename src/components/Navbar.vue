<template>
  <header>
      <nav>
          <img :src=" require('@/assets/img/dc-logo.png') " alt="Logo">

          <ul id="container_link">
                <li class="link" v-for="link,i of links" :key="i">
                    <a :href="link.link">{{ link.text }}</a>
                </li>
          </ul>
      </nav>
      <div id="black">
        <h2> Content goes here </h2>
      </div>
  </header>
</template>

<script>
export default {
    name: 'Navbar',
    data: () => ({
        links: [
            {
                link: "#",
                text: "CHARACTERS"
            },
            {
                link: "#",
                text: "COMICS"
            },
            {
                link: "#",
                text: "MOVIES"
            },
            {
                link: "#",
                text: "TV"
            },
            {
                link: "#",
                text: "GAMES"
            },
            {
                link: "#",
                text: "COLLECTIBLES"
            },
            {
                link: "#",
                text: "VIDEOS"
            },
            {
                link: "#",
                text: "FANS"
            },
            {
                link: "#",
                text: "NEWS"
            },
            {
                link: "#",
                text: "SHOP"
            }
            
        ]
    })
}
</script>

<style>

nav{
    display:flex;
    justify-content: space-around;
    height: 10vh;
}

#container_link{
    display: flex;
    list-style-type: none;
    font-size: 15px;
    line-height:9vh;
}

a{
    text-decoration: none;
    padding:15px;
    color: black;
}

nav > img{
margin-top: 10px;
}

#black{
    background-color: black;
    height:12vh;
}

#black > h2{
    color:#ffffff;
    line-height:12vh;
    margin-left:120px;
}
</style>