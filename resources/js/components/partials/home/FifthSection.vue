<template>
    <section class="overflow-hidden ">
        <!-- testimonials slider -->
        <Splide :has-track="false"  :options="options" class="px-4 pt-12">
            <div class="container mx-auto flex items-center justify-between">
                <h2 class="text-2xl lg:text-4xl xl:text-5xl font-bold">
                    <span>What our clients say</span><br>
                    <span>about our services</span>
                </h2>
                <div class="custom-slide-arrows splide__arrows flex items-center gap-x-4" style="position: relative">
                    <button class="splide__arrow splide__arrow--prev text-black hover:shadow-lg">
                        <svg  width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M13 24L21 16L13 8" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                        </svg>
                    </button>
                    
                    <button class="splide__arrow splide__arrow--next  text-black hover:shadow-lg">
                       <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M13 24L21 16L13 8" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                        </svg>
                    </button>
                </div>
            </div>
            <!-- slider wrapper -->
            <div class="slide-wrapper container mx-auto mt-12">
                <div class="splide__track pt-16 pb-8" ref="splideTrack">
                    <ul class="splide__list">
                        <li class="splide__slide w-full max-w-full h-auto">
                            <TestimonialCard class="testimonial-card h-full">
                                <template #img>
                                    <img src="/assets/images/home/testimonials/json-wong.webp" alt="" srcset="">
                                </template>
                                <template #name>
                                    Jason Wong
                                </template>
                                <template #role>
                                    CEO at Omnicharge
                                </template>
                                <template #testimony>
                                    The work of the Prospecta team was very productive. We were especially impressed by the deep research - it seemed that Prospecta experts started speaking our brand’s language after delving into our style guidelines and investigating them for a while.
                                </template>
                            </TestimonialCard>
                        </li>
                        <li class="splide__slide w-full max-w-full h-auto">
                            <TestimonialCard class="testimonial-card h-full" >
                                <template #img>
                                    <img src="/assets/images/home/testimonials/audrey-wyrick.webp" alt="" srcset="">
                                </template>
                                <template #name>
                                    Audrey Wyrick
                                </template>
                                <template #role>
                                    Senior Product Marketing Manager at Cengage Group
                                </template>
                                <template #testimony>
                                    Prospecta proved their expertise by exceeding expectations and target goals while increasing brand awareness. The Prospecta team scheduled calls with 10,000+ employee size organizations, which brought us a lot of great conversations that are actively moving forward.
                                </template>
                            </TestimonialCard>
                        </li>
                        <li class="splide__slide w-full max-w-full h-auto">
                            <TestimonialCard class="testimonial-card h-full" >
                                <template #img>
                                    <img src="/assets/images/home/testimonials/maria-barroca.webp" alt="" srcset="">
                                </template>
                                <template #name>
                                    Maria Barroca
                                </template>
                                <template #role>
                                    Global Campaigns Manager at OutSystems
                                </template>
                                <template #testimony>
                                    The results exceeded our expectations. Prospecta went above and beyond to adapt to our processes, ensuring a smooth workflow. Their team has been doing its best - it delivered more than 20 appointments in a month and a half.
                                </template>
                            </TestimonialCard>
                        </li>
                        <li class="splide__slide w-full max-w-full h-auto">
                            <TestimonialCard class="testimonial-card h-full" >
                                <template #img>
                                    <img src="/assets/images/home/testimonials/brendan-walsh.webp" alt="" srcset="">
                                </template>
                                <template #name>
                                    Brendan Walsh
                                </template>
                                <template #role>
                                    Co-Founder & Principal at Mole Street
                                </template>
                                <template #testimony>
                                    They’ve been consistently booking 5–7 sales-qualified appointments for us every month. We just closed one of our largest contracts based on their lead research yesterday. They are the real deal. I can’t say enough good things about Prospecta.
                                </template>
                            </TestimonialCard>
                        </li>
                        <li class="splide__slide w-full max-w-full h-auto">
                            <TestimonialCard class="testimonial-card h-full" >
                                <template #img>
                                    <img src="/assets/images/home/testimonials/tony-rozanski.webp" alt="" srcset="">
                                </template>
                                <template #name>
                                    Tony Rozanski
                                </template>
                                <template #role>
                                    Head of Finance and Operations at EBCO Trends
                                </template>
                                <template #testimony>
                                    Prospecta superpower is how effectively their experts use software to get the actionable data. They don’t act intuitively but stay data-driven and consistent. They know what they need to do and when.
                                </template>
                            </TestimonialCard>
                        </li>
                        <li class="splide__slide w-full max-w-full h-auto">
                            <TestimonialCard class="testimonial-card h-full" >
                                <template #img>
                                    <img src="/assets/images/home/testimonials/peter-sher.webp" alt="" srcset="">
                                </template>
                                <template #name>
                                    Peter Sher
                                </template>
                                <template #role>
                                    Vice President of Sales at Driveline
                                </template>
                                <template #testimony>
                                    Among the total number of calls, we have a large percentage of scheduled meetings, interested prospects, and even closed deals. The result is impressive!
                                </template>
                            </TestimonialCard>
                        </li>
                    </ul>
                </div>
            </div>
        </Splide>
         
        
    </section>
</template>
<script>
// Default theme
import '@splidejs/vue-splide/css';

import TestimonialCard  from '../../UI/TestimonialCard.vue'
import { Splide } from '@splidejs/vue-splide';

export default {
    components:{
        TestimonialCard,
        Splide,
    },
    data() {
      return{
        options:{
            rewind:false,
            perMove: 1,
            arrows:true,
            pagination: false,
            type  : 'loop',
            drag:true,
            gap:'87.6px',
            keyboard:'global',
            

            breakpoints: {
                1280: {
                    rewind:false,
                    perMove: 1,
                    arrows:true,
                    pagination: false,
                    type  : 'loop',
                    drag:true,
                    gap:'32px',
                    keyboard:'global',
                    
                },
                1024: {
                    rewind:false,
                    perMove: 1,
                    arrows:false,
                    pagination: false,
                    type  : 'slide',
                    drag:false,
                    gap:'16px',
                    keyboard:false,
                }
            },
        },
        
      }
    },
    methods:{
        scrolling(event){
            console.log(event.keyCode);
            let scrollOffset = 0
            if (event.keyCode === 37) {
                scrollOffset = -this.$refs.splideTrack.offsetWidth
            } else if (event.keyCode === 39) {
                scrollOffset = this.$refs.splideTrack.offsetWidth
            }
            this.$refs.splideTrack.scrollBy({
                top: 0,
                left: scrollOffset,
                behavior: "smooth",
            });
        },
        scrollRight(){
            this.$refs.splideTrack.scrollBy({
                top: 0,
                left: -this.$refs.splideTrack.offsetWidth,
                behavior: "smooth",
            });
        },

    },
    mounted() {
        // window.addEventListener("keydown", this.scrolling);
    },
    
   
}
</script>

<style scoped>
.splide__track{
    overflow-x:scroll;
    scroll-behavior: smooth;
    scroll-snap-type: x mandatory;
}

.splide__arrow{
    position: relative;
    left: 0;
    right: 0;
    padding: 12px;
    background: white;
    width: auto;
    height: auto;
    transform: translateY(0);
}
.splide__arrow--next svg {
        transform: scaleX(1) !important;
}
.splide__arrow--prev svg {
        transform: scaleX(1) rotate(-180deg) !important;
}
.splide__arrow svg {
    fill: none;
    height: 2rem;
    width: 2rem;
}

@media (min-width: 1000px) {
    .splide__track{
        /* overflow-x:hidden; */
        overflow: visible;
        overflow-x:visible;
    }
    .testimonial-card {
        @apply pr-0;
    }
    .splide__slide{
        width: 544px !important;
    }
}

.splide__track::-webkit-scrollbar {
    background-color: transparent;
    height: 6px;
}

.splide__track::-webkit-scrollbar-thumb {
    background-color: #0000001a;
    border-radius: 100px;
}

.splide__track::-webkit-scrollbar-track {
    background-color: #ebebeb;
    border-radius: 100px;
}
</style>

