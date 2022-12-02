<script>
export default{
    data(){
        return {
            arrayNavbar: ["CHARACTERS", "COMICS", "MOVIES", "TV", "GAMES", "COLECTIBLES", "VIDEO", "FANS", "NEWS", "SHOP"],
            
        }
    },
    methods: {
        cicloArray() {
            for (let i = 0; i < this.arrayNavbar.length; i++){
                this.arrayNavbar.join(" ");

            }
            console.log(this.cicloArray);
        }
    }

};
</script>

<template>
    <div class="container">
        <div>
            <img src="public/img/dc-logo.png" alt="">
        </div>
        <div class="navbar" v-for="(element, i) in arrayNavbar">
            {{element}}
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../styles/general.scss";

.container{
    width: 920px;
    display: flex;
}

.navbar{
    display: flex;
    justify-content: space-between;
}

img{
    display: block;
    width: 100%;
    object-fit: contain;
}
</style>