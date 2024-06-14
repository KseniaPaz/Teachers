<template>
    <div>
        <div class="carousel">
            <div class="slider" :style="{ 'margin-left': '-' + (40 * currentSlideIndex) + '%' }">
                <TeUser
                v-for="item in carousel_data" :key="item.id"
                :userData="item"
            
                />            
            </div>
            
        </div>
        <div class="button__box">
                <img @click="prevSlide" src="../assets/img/Arrow - Left Circle.svg" alt="left">
                <img @click="nextSlide" src="../assets/img/Arrow - Right Circle.svg" alt="right">
        </div>
    </div>
    
</template>

<script>
    import TeUser from './TeUser.vue' 

    export default {
        name: 'TeCarousel',
        components: {
            TeUser
        },

        props: {
            carousel_data: {
                type: Array,
                }
        },

        data() {
            return {
                currentSlideIndex: 0
            }
        },

        methods: {
            prevSlide() {
                if (this.currentSlideIndex > 0) {
                    this.currentSlideIndex--
                    console.log(this.currentSlideIndex);
                }
                
            },
            nextSlide() {
                if (this.currentSlideIndex >= this.carousel_data.length - 3) {
                    this.currentSlideIndex = 0
                } else {
                   this.currentSlideIndex++
                    console.log(this.currentSlideIndex); 
                }
                
            }

        },
    }
</script>

<style lang="scss" scoped>
    .carousel {
        overflow-x: hidden;
        display: flex;
    }

    .slider {
        display: flex;
        max-width: 360px;
        gap: 20px;
        transition: all ease .5s;
    }

    .button__box {
        display: flex;
        margin-top: 60px;
        gap: 10px;
        justify-content: flex-end;
      }

</style>