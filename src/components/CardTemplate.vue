<template>
    <div>
        <div class="container">
            <div class="card-custom-style">
                <img :src="thumb" :alt="`Cover img ${series}`">
            </div>
            <div>
                <p class="text-card-custom-style">{{ series.toUpperCase()    }}</p>
            </div>

        </div>
    </div>
</template>

<script>
export default {
    props: {
        thumb: String,
        price: String,
        series: String,
        type: String,
    },
    data() {
        return{
        }
    },

}
</script>

<style lang="scss" scoped>
.container {
        transition: opacity .2s ease-in-out;
    &:hover {
        opacity: .6;
    }
}

.card-custom-style {
    height: 180px;
    width: 180px;
    border-radius: 0;
    overflow: hidden;
    cursor: pointer;


    img {
        height: 100%;
        width: 100%;
    }
}

    .text-card-custom-style{
        color: white;
        max-width: 180px;
        font-size: .7rem;
        padding-top: .8rem;
        font-weight: 300;
        cursor: pointer;
    }   

</style>