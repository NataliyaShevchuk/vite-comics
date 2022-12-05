<script>
    export default {
        props: {
            cards: {
                type: Object,
                required: true,
            }
        },
        data() {
            return {
                cardTitle: this.cards.series.toUpperCase(),
            }
        }
    }
</script>





<template>
    <div class="card">
        <img class="card-img" :src="cards.thumb" alt="cover of a comic">
        <div class="card-title">
            <h6 class="comic-title"> {{cardTitle}} </h6>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../styles/general.scss" as *;

.card{
    padding: 1rem;

}
.card-img{
    aspect-ratio: 1 / 1;
    object-fit: cover;
    object-position: top;

    &:hover{
        opacity: 50%;
        cursor: pointer;
        
    }
}

.comic-title{
    color: white;
    padding: 1rem 0;
    font-weight: 300;
}


</style>