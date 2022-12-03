<script>
export default{
    data(){
        return {
            arrayNavbar: [
                {
                    navLink: "CHARACTERS",
                    navOption: "See all",
                    navOptionTwo: "First superHeroes",
                },
                {
                    navLink: "COMICS",
                    navOption: "See all",
                    navOptionTwo: "First superHeroes",
                },
                {
                    navLink: "MOVIES",
                    navOption: "See all",
                    navOptionTwo: "First superHeroes",
                },
                {
                    navLink: "TV",
                    navOption: "See all",
                    navOptionTwo: "First superHeroes",
                },
                {
                    navLink: "GAMES",
                    navOption: "See all",
                    navOptionTwo: "First superHeroes",
                },
                {
                    navLink: "COLLECTIBLES",
                    navOption: "See all",
                    navOptionTwo: "First superHeroes",
                },
                {
                    navLink: "VIDEOS",
                    navOption: "See all",
                    navOptionTwo: "First superHeroes",
                },
                {
                    navLink: "FANS",
                    navOption: "See all",
                    navOptionTwo: "First superHeroes",
                },
                {
                    navLink: "NEWS",
                    navOption: "See all",
                    navOptionTwo: "First superHeroes",
                },
                {
                    navLink: "SHOP",
                    navOption: "See all",
                    navOptionTwo: "First superHeroes",
                }
            ]
            
        }
    },
    methods: {
        cicloArray() {
            for (let i = 0; i < this.arrayNavbar; i++){


            }
            console.log(this.cicloArray);
        }
    }

};
</script>

<template>
    <nav class="white-bg">
        <div class="container">
            <div class="img-container">
                <img src="" alt="">
            </div>

            <ul>
                <li v-for="(element, index) in arrayNavbar">
                    <a href="#">
                        {{element.navLink}}
                    </a>
                </li>
            </ul>
        </div>

    </nav>
</template>

<style scoped lang="scss">
@use "../styles/general.scss" as *;

.container{
    width: 920px;
    display: flex;
}


img{
    display: block;
    width: 100%;
    object-fit: contain;
}

.white-bg{
    width: 100%;
    background-color: white;
    color: $color-secondary;
    height: 100px;
}
nav {
    ul {
        display: flex;
        li {
            list-style: none;
        } 
        a{
            text-decoration: none;
            padding: 1rem;
            color: $color-secondary;
        }
    }
}
</style>