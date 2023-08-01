<template>
<div class="px-4">

    <div @click="$emit('changeComponent','SmallScreenMenu')" class="mt-4 flex items-center gap-x-1 text-[#8f8f8f] text-xs cursor-pointer w-fit">
        <svg class="w-3  h-3 -rotate-180" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
        </svg>
        <span class="">What we do</span> 
    </div>

    <div v-accordion class="mt-4 accordion bg-[#fbfbfb] rounded-sm px-6 py-2 flex flex-col divide-y">
        <!-- accordion-item -->
        <div class="accordion-item py-4">
            <div class="accordion-header w-full text-xl flex items-center justify-between">
                <div class="flex items-center gap-x-2">
                    <svg class="w-6 h-6" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" width="20" height="20" fill="none">
                        <path stroke="#FF5E00" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M15 5.967a.504.504 0 0 0-.158 0 2.144 2.144 0 0 1-2.067-2.15c0-1.192.958-2.15 2.15-2.15a2.15 2.15 0 0 1 .075 4.3ZM14.142 12.034c1.141.191 2.4-.009 3.283-.6 1.175-.784 1.175-2.067 0-2.85-.892-.592-2.167-.792-3.308-.592M4.975 5.967a.504.504 0 0 1 .159 0A2.144 2.144 0 0 0 7.2 3.817c0-1.192-.958-2.15-2.15-2.15a2.15 2.15 0 0 0-.075 4.3ZM5.834 12.034c-1.142.191-2.4-.009-3.284-.6-1.175-.784-1.175-2.067 0-2.85.892-.592 2.167-.792 3.309-.592M10 12.192a.506.506 0 0 0-.158 0 2.144 2.144 0 0 1-2.067-2.15c0-1.192.958-2.15 2.15-2.15a2.15 2.15 0 0 1 2.15 2.15c-.008 1.166-.925 2.116-2.075 2.15ZM7.575 14.817c-1.175.783-1.175 2.067 0 2.85 1.333.891 3.517.891 4.85 0 1.175-.784 1.175-2.067 0-2.85-1.325-.883-3.517-.883-4.85 0Z"/>
                    </svg>
                    <span class="text-lg font-semibold">Lead Generation Services</span> 
                </div>
                <svg class="chevron w-6 h-6 text-orange-600" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                </svg>
            </div>
            <div class="accordion-content flex flex-col mt-4 text-sm font-medium">
                <a href="#" class="py-3">Appointment setting</a>
                <a href="#" class="py-3">Demand generation</a>
                <a href="#" class="py-3">Cold email outreach</a>
                <a href="#" class="py-3">Sales development</a>
            </div>
        </div>
        <!-- accordion-item -->
        <div class="accordion-item py-4">
            <div class="accordion-header w-full text-xl flex items-center justify-between">
                <div class="flex items-center gap-x-2">
                    <svg  class="w-6 h-6" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" width="20" height="20" fill="none">
                        <path stroke="#FF5E00" stroke-linecap="round" stroke-linejoin="round" stroke-miterlimit="10" stroke-width="1.5" d="M9.996 12.648a2.649 2.649 0 1 0 0-5.297 2.649 2.649 0 0 0 0 5.297Z"/>
                        <path stroke="#FF5E00" stroke-linecap="round" stroke-linejoin="round" stroke-miterlimit="10" stroke-width="1.5" d="M1.167 10.776V9.222c0-.918.75-1.677 1.677-1.677 1.598 0 2.252-1.13 1.448-2.516a1.677 1.677 0 0 1 .618-2.287l1.528-.874c.697-.415 1.598-.168 2.013.53l.097.168c.794 1.386 2.101 1.386 2.904 0l.098-.168c.414-.698 1.315-.945 2.012-.53l1.528.874a1.677 1.677 0 0 1 .618 2.287c-.803 1.386-.15 2.516 1.448 2.516.918 0 1.677.75 1.677 1.677v1.554c0 .918-.75 1.678-1.677 1.678-1.598 0-2.251 1.13-1.448 2.516.459.803.185 1.827-.618 2.287l-1.527.874c-.698.415-1.599.167-2.013-.53l-.098-.168c-.794-1.386-2.1-1.386-2.904 0l-.097.168c-.415.697-1.316.945-2.013.53l-1.528-.874a1.677 1.677 0 0 1-.618-2.287c.804-1.386.15-2.516-1.448-2.516-.927 0-1.677-.76-1.677-1.678Z"/>
                    </svg>
                    <span class="text-lg font-semibold">Other services</span> 
                </div>
                <svg class="chevron w-6 h-6 text-orange-600" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                </svg>
            </div>
            <div class="accordion-content flex flex-col mt-4 text-sm font-medium">
                <a href="#" class="py-3">LinkedIn marketing</a>
                <a href="#" class="py-3">CRM consulting</a>
                <a href="#" class="py-3">Sales enablement</a>
                <a href="#" class="py-3">Our Process</a>
            </div>
        </div>
    </div>

    <!-- banner -->
    <div class="mt-4 min-h-[17.4rem] rounded-2xl overflow-hidden flex relative">
        <img class="z-0 absolute top-0 left-0 w-full h-full object-cover object-left-top" src="/assets/images/header/what-we-do-banner-background.webp">
        <div class="z-10  flex flex-col gap-y-6 px-4 py-8">
            <div class="flex flex-col gap-y-3">
                <h1 class="text-[1.75rem] font-bold leading-10">
                    <div>GET <span class="text-orange-600">20 PILOT</span> </div>
                    <div><span class="text-orange-600">Leads</span> FOR FREE</div>
                </h1>
                <div class="text-sm">Want to see our work in action? Request 20 complimentary leads to make sure it's 100% fit to your ICP</div>
            </div>
            <a href="#" class="w-fit flex items-center gap-x-2 text-[#292929] bg-white  hover:text-orange-600 rounded-md py-2.5 pl-4 pr-2.5">
                <span class="text-sm font-semibold">Get my Leads</span>
                <svg class="w-4 h-4" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                </svg>
            </a>
        </div>
        
    </div>

</div>
</template>