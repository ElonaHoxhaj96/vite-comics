<script>
export default {
    name: 'AppHeader',
    date(){
    return{
        activeIndex: 0,
        linksMenu:[
          { 
            text: 'CHARACTER',
            url: '#',
          },
          { 
            text: 'MOVIES',
            url: '#'
          },
          { 
            text: 'TV',
            url: '#'
          },
          { 
            text: 'GAMES',
            url: '#'
          },
          { 
            text: 'COLLECTIBLES',
            url: '#'
          },
          { 
            text: 'VIDEOS',
            url: '#'
          },
          { 
            text: 'FANS',
            url: '#'
          },
          { 
            text: 'NEWS',
            url: '#'
          },
          { 
            text: 'SHOP',
            url: '#'
          },
        ],

    }
},
methods: {
  toggleNav(index) {
    this.activeIndex = index;
    console.log(this.toggleNav);
  }
}
}
</script>


<template> 
    <header>
        <nav>
            <div>
                <img src="../assets/dc-logo.png" alt="logo">
            </div>
            <ul>
                <li v-for="(link, index) in linksMenu" :key="index">
                    <a :href="link.url" class=":hover">{{link.text}}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
    nav{
        display: flex;
        justify-content: space-around;
        align-items: center;
    }
    ul{
        display: flex;
        gap: 1rem;
    }
    li{
       list-style: none;
       :hover{
            border-bottom: solid 0.2rem blue;
            }
       a{
        text-decoration: none;
        color: rgb(88, 88, 88);
        font-weight: bold;
        padding-bottom: 2.4rem; 
       }
    }

</style>