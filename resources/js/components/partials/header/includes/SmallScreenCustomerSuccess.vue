<template>
<div class="px-4">

    <div @click="$emit('changeComponent','SmallScreenMenu')" class="mt-4 flex items-center gap-x-1 text-[#8f8f8f] text-xs cursor-pointer w-fit">
        <svg class="w-3  h-3 -rotate-180" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
        </svg>
        <span class="">Customer success</span> 
    </div>

    <!-- accordion -->
    <div v-accordion class="mt-4 accordion bg-[#fbfbfb] rounded-sm px-6 py-2 flex flex-col divide-y">
        <!-- accordion item -->
        <div class="accordion-item py-4">
            <div class="accordion-header w-full text-xl flex items-center justify-between">
                <div class="flex items-center gap-x-2">
                    
                    <svg class="w-6 h-6" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" width="20" height="20" fill="none">
                        <path stroke="#FF5E00" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="m13.75 7.917-3.5 3.5-1.333-2-2.667 2.667"/>
                        <path stroke="#FF5E00" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M12.084 7.917h1.666v1.667"/>
                        <path stroke="#FF5E00" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M7.5 18.334h5c4.166 0 5.833-1.667 5.833-5.834v-5c0-4.166-1.666-5.833-5.833-5.833h-5c-4.167 0-5.833 1.667-5.833 5.833v5c0 4.167 1.666 5.834 5.833 5.834Z"/>
                    </svg>
                    
                    <span class="text-lg font-semibold">Customer stories</span> 
                </div>
                <svg class="chevron w-6 h-6 text-orange-600" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                </svg>
            </div>
            <div class="accordion-content flex flex-col mt-4 text-sm font-medium">
                <a href="#" class="py-3">Case studies</a>
                <a href="#" class="py-3">Reviews & testimonials</a>
                <a href="#" class="py-3">ROI calculator</a>
            </div>
        </div>
        <!-- accordion item -->
        <div class="accordion-item py-4">
            <div class="accordion-header w-full text-xl flex items-center justify-between">
                <div class="flex items-center gap-x-2">
                    <svg  class="w-6 h-6" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" width="20" height="20" fill="none">
                        <path stroke="#FF5E00" stroke-linecap="round" stroke-linejoin="round" stroke-miterlimit="10" stroke-width="1.5" d="M9.996 12.648a2.649 2.649 0 1 0 0-5.297 2.649 2.649 0 0 0 0 5.297Z"/>
                        <path stroke="#FF5E00" stroke-linecap="round" stroke-linejoin="round" stroke-miterlimit="10" stroke-width="1.5" d="M1.167 10.776V9.222c0-.918.75-1.677 1.677-1.677 1.598 0 2.252-1.13 1.448-2.516a1.677 1.677 0 0 1 .618-2.287l1.528-.874c.697-.415 1.598-.168 2.013.53l.097.168c.794 1.386 2.101 1.386 2.904 0l.098-.168c.414-.698 1.315-.945 2.012-.53l1.528.874a1.677 1.677 0 0 1 .618 2.287c-.803 1.386-.15 2.516 1.448 2.516.918 0 1.677.75 1.677 1.677v1.554c0 .918-.75 1.678-1.677 1.678-1.598 0-2.251 1.13-1.448 2.516.459.803.185 1.827-.618 2.287l-1.527.874c-.698.415-1.599.167-2.013-.53l-.098-.168c-.794-1.386-2.1-1.386-2.904 0l-.097.168c-.415.697-1.316.945-2.013.53l-1.528-.874a1.677 1.677 0 0 1-.618-2.287c.804-1.386.15-2.516-1.448-2.516-.927 0-1.677-.76-1.677-1.678Z"/>
                    </svg>
                    <span class="text-lg font-semibold">Industries</span> 
                </div>
                <svg class="chevron w-6 h-6 text-orange-600" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                </svg>
            </div>
            <div class="accordion-content flex flex-col mt-4 text-sm font-medium">
                <a href="#" class="py-3">Finance</a>
                <a href="#" class="py-3">Manufacturing</a>
                <a href="#" class="py-3">Healthcare</a>
                <a href="#" class="py-3 flex items-center gap-x-1">
                    <span>See all</span>
                    <svg class="w-4 h-4" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M4.5 12h15m0 0l-6.75-6.75M19.5 12l-6.75 6.75" />
                    </svg>
                </a>
            </div>
        </div>
    </div>
    <!-- banner -->
    <div class="mt-4 min-h-[17.4rem] rounded-2xl overflow-hidden flex relative">
        <img class="z-0 absolute top-0 left-0 w-full h-full object-cover object-center" src="/assets/images/header/customer-success-banner-background.webp">
        <div class="z-10  flex flex-col gap-y-6 px-6 py-8">
            <div>
                    <h2 class="text-2xl font-bold leading-none italic text-orange-600">
                        B2B COLD EMAIL
                    </h2>
                    <h1 class="text-[2.125rem] font-bold leading-none italic">
                        OUTREACH BENCHMARKS
                    </h1>
            </div>
            <a href="#" class="w-fit flex items-center gap-x-2 text-white  hover:bg-orange-600/70 bg-orange-600 rounded-md py-2.5 px-4">
                <span class="text-sm font-semibold">Get the report</span>
            </a>
        </div>
        
    </div>

    

</div>
</template>