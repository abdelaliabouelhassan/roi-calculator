<template>
    <section class="py-12 flex flex-col gap-y-6 lg:pb-32 lg:pt-6 xl:pb-40">
        <!-- brand slide 1 -->
        <Splide ref="slide1" :options="options1" :extensions="extensions" class="px-4 lg:hidden">
            <SplideSlide class="min-w-full lg:min-w-fit lg:w-fit flex items-center">
                <!--  bob -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/bob.svg" alt="" srcset="">
                </div>
                <!-- ebanx -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/ebanx.svg" alt="" srcset="">
                </div>
                <!-- ordway -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/ordway.svg" alt="" srcset="">
                </div>
                <!-- citcon -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/citcon.png" alt="" srcset="">
                </div>
                <!-- cemtrex -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/cemtrex.svg" alt="" srcset="">
                </div>
                
            </SplideSlide>
            <!-- duplicate slide -->
            <SplideSlide class="min-w-full flex items-center ">
                <!--  bob -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/bob.svg" alt="" srcset="">
                </div>
                <!-- ebanx -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/ebanx.svg" alt="" srcset="">
                </div>
                <!-- ordway -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/ordway.svg" alt="" srcset="">
                </div>
                <!-- citcon -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/citcon.png" alt="" srcset="">
                </div>
                <!-- cemtrex -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/cemtrex.svg" alt="" srcset="">
                </div>
            </SplideSlide>
            
        </Splide>
        <!-- brand slide 2-->
        <Splide ref="slide2" :options="options2" :extensions="extensions" class="px-4 lg:hidden">
            <SplideSlide class="min-w-full flex items-center">
                <!--  bornbred -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/bornbred.svg" alt="" srcset="">
                </div>
                <!-- citrusad -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/citrusad.svg" alt="" srcset="">
                </div>
                <!-- berkeley -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/berkeley.png" alt="" srcset="">
                </div>
                <!-- mole-street -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/mole-street.svg" alt="" srcset="">
                </div>
                <!-- digital-knights -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/digital-knights.svg" alt="" srcset="">
                </div>
                
            </SplideSlide>
            <SplideSlide class="min-w-full flex items-center">
                <!--  bornbred -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/bornbred.svg" alt="" srcset="">
                </div>
                <!-- citrusad -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/citrusad.svg" alt="" srcset="">
                </div>
                <!-- berkeley -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/berkeley.png" alt="" srcset="">
                </div>
                <!-- mole-street -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/mole-street.svg" alt="" srcset="">
                </div>
                <!-- digital-knights -->
                <div class="w-32 h-16 scale-[0.8] mx-4 brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/digital-knights.svg" alt="" srcset="">
                </div>
                
            </SplideSlide>
            
        </Splide>

        <!-- brand slide 3-->
        <Splide ref="slide3" :options="options2" :extensions="extensions" class="px-4 hidden lg:block">
            
                <!--  bob -->
            <SplideSlide class="scale-[0.6] brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/bob.svg" alt="" srcset="">
            </SplideSlide>
                <!-- ebanx -->
            <SplideSlide class="scale-[0.8] brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/ebanx.svg" alt="" srcset="">
            </SplideSlide>
                <!-- ordway -->
            <SplideSlide class="scale-[0.8] brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/ordway.svg" alt="" srcset="">
            </SplideSlide>
                <!-- citcon -->
            <SplideSlide class="scale-[0.8] brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/citcon.png" alt="" srcset="">
            </SplideSlide>
                <!-- cemtrex -->
            <SplideSlide class="scale-[0.8] brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/cemtrex.svg" alt="" srcset="">
            </SplideSlide>
                



            <SplideSlide class="scale-[0.8] brand-filter">
                <img class="w-full h-full object-contain" src="assets/images/home/brands/bornbred.svg" alt="" srcset="">
            </SplideSlide>
                <!-- citrusad -->
            <SplideSlide class="scale-[0.8] brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/citrusad.svg" alt="" srcset="">
            </SplideSlide>
                <!-- berkeley -->
            <SplideSlide class="scale-[0.8] brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/berkeley.png" alt="" srcset="">
            </SplideSlide>
                <!-- mole-street -->
            <SplideSlide class="scale-[0.8] brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/mole-street.svg" alt="" srcset="">
            </SplideSlide>
                <!-- digital-knights -->
            <SplideSlide class="scale-[0.8] brand-filter">
                    <img class="w-full h-full object-contain" src="assets/images/home/brands/digital-knights.svg" alt="" srcset="">
            </SplideSlide>
                
            
            
            
        </Splide>
    </section>
</template>

<script>
// Default theme
import '@splidejs/vue-splide/css';

import TestimonialCard  from '../../UI/TestimonialCard.vue'
import { Splide, SplideSlide } from '@splidejs/vue-splide';
import { AutoScroll } from '@splidejs/splide-extension-auto-scroll';

export default {
    components:{
        TestimonialCard,
        Splide
    },
    data() {
      return{
            extensions:{
                AutoScroll
            },
            options1:{
                rewind:true,
                type   : 'loop',
                drag   : true,
                focus  : 'center',
                arrows:false,
                autoWidth:true,
                pagination:false,
                autoScroll: {
                    speed: 0.5,
                    autostart:true,
                    pauseOnHover:false
                },
            },
            options2:{
                rewind:true,
                type   : 'loop',
                drag   : true,
                focus  : 'center',
                arrows:false,
                autoWidth:true,
                pagination:false,
                autoScroll: {
                    speed: -0.5,
                    autostart:true,
                    pauseOnHover:false
                },
            }
        }
    },
    mounted() {
        // this.$refs.slide1
        setTimeout(() => {
            
            console.log(this.$refs.slide1);
        }, 3000);
    },
    
    
    
   
}
</script>

<style scoped>
.brand-filter {
    transition: all 150ms ease-in-out;
    filter: invert(41%) sepia(3%) saturate(17%) hue-rotate(30deg) brightness(94%) contrast(88%);
}
.brand-filter:hover {
    filter: none;
}
@media (min-width: 1024px) {
    .splide__slide {
        width: 10rem;
        height: 5rem;
        margin: 0 16px;
    }
}


</style>