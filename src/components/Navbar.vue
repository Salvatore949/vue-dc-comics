<template>
  <header>
      <nav>
          <img :src=" require('@/assets/logo.png') " alt="Logo">
          <!-- <img :src=" require('@/assets/img/avatar_1.jpg') " alt="Logo"> -->

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
    align-items: center;
    list-style-type: none;
    font-size: 15px;
}

a{
    text-decoration: none;
    padding:15px;
    color: black;
}

nav > img{
    display: flex;
    align-items: center;
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