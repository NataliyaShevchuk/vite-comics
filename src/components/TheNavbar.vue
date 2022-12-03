<script>
export default{
    data(){
        return {
            logoImg: "dc-logo.png",
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
                <img :src="('/img/' + logoImg)" alt="logo della dc">
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
    justify-content: space-between;
    align-items: center;
    margin: auto;
    padding: 10px 0;

}

.img-container{
    margin-right: 1rem;
    text-align: center;
    width: 60px;
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
        margin-left: 6rem;
        li {
            list-style: none;
            font-size: 12px;
            font-weight: 500;
        } 
        a{
            text-decoration: none;
            padding: 1rem;
            padding-bottom: 3.2rem;
            color: $color-secondary;

            &:hover{
                border-bottom: 4px solid $hover-color;
                color: $hover-color;
            }
        }

    }
}
</style>