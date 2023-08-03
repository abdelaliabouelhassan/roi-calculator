<template>
    <section class="flex flex-col items-center gap-y-6 container mx-auto xl:max-w-[67.25rem] px-4 py-12 lg:pt-12 lg:pb-32 lg:flex-row lg:justify-between lg:gap-x-24 
            xl:pt-16 xl:pb-40">
        
        <div class="flex flex-col gap-y-6 w-full ">
            <h1 class="text-2xl font-bold lg:text-[2rem]">Timeline of appointment setting results</h1>
            <p class="lg:text-lg">One of the most common questions our clients ask is how quickly they can expect the results from their outbound efforts. Check out the video, where our sales expert explains how the duration of your campaign can impact your ROI. We break down the differences between running campaigns for 3, 6, and 12 months with Prospecta.</p>
        </div>

        <div class="z-10 relative   w-full max-w-[496px] h-[320px] ">
            
            <div v-if="!playVideo" class="z-10 w-full h-full flex flex-col items-center justify-center">
                <!-- video background -->
                <div class="z-0 w-full h-full absolute top-0 left-0 rounded-2xl overflow-hidden border border-white">
                    <img class="w-full h-full object-cover object-left-top" src="/assets/images/home/third-section/video-bg.webp" alt="" srcset="">
                </div>
                <button @click="playVideo = !playVideo" class="z-10 rounded-full w-[200px] h-16 flex items-center justify-center gap-x-4 bg-black/70">
                    <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <circle cx="16" cy="16" r="16" fill="white" fill-opacity="0.2"/>
                        <g filter="url(#filter0_b_19874_200464)">
                        <path d="M14.1306 11.2205C13.2301 10.7033 12.5 11.127 12.5 12.166V19.8333C12.5 20.8733 13.2301 21.2964 14.1306 20.7797L20.8244 16.9364C21.7252 16.4191 21.7252 15.5809 20.8244 15.0637L14.1306 11.2205Z" fill="white"/>
                        </g>
                        <defs>
                        <filter id="filter0_b_19874_200464" x="4.5" y="3" width="25" height="26" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
                        <feFlood flood-opacity="0" result="BackgroundImageFix"/>
                        <feGaussianBlur in="BackgroundImageFix" stdDeviation="4"/>
                        <feComposite in2="SourceAlpha" operator="in" result="effect1_backgroundBlur_19874_200464"/>
                        <feBlend mode="normal" in="SourceGraphic" in2="effect1_backgroundBlur_19874_200464" result="shape"/>
                        </filter>
                        </defs>
                    </svg>
                    <span class="text-white font-semi-bold">Watch video</span>
                </button>
            </div>
            <div v-else>
                <iframe class="w-full h-full rounded-3xl overflow-hidden" style="height:315px;" src="https://www.youtube.com/embed/MDSlF1l5w40?autoplay=1" frameborder="0"></iframe>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            playVideo:false
        }
    },
}
</script>
