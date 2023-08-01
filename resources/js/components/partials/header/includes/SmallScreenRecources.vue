<template>
<div class="px-4">

    <div @click="$emit('changeComponent','SmallScreenMenu')" class="mt-4 flex items-center gap-x-1 text-[#8f8f8f] text-xs cursor-pointer w-fit">
        <svg class="w-3  h-3 -rotate-180" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
        </svg>
        <span class="">Resources</span> 
    </div>

    <div v-accordion class="mt-4 accordion bg-[#fbfbfb] rounded-sm px-6 py-2 flex flex-col divide-y">
        <!-- accordion-item -->
        <div class="accordion-item py-4">
            <div class="accordion-header w-full text-xl flex items-center justify-between">
                <div class="flex items-center gap-x-2">
                    
                    <svg class="w-6 h-6" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" width="20" height="20" fill="none">
                        <path fill="#FF5E00" fill-rule="evenodd" d="M14.167 17.583a.917.917 0 1 0 0-1.833H5.833a.917.917 0 1 0 0 1.833h8.334Zm-9.304-3.13a2.417 2.417 0 0 0 .97 4.63h8.334a2.417 2.417 0 0 0 .97-4.63l1.172-3.641a4.037 4.037 0 0 0-.492-3.828l-.015-.022-4.415-5.36c-.677-.914-2.097-.914-2.773 0l-4.416 5.36-.015.022a4.037 4.037 0 0 0-.491 3.828l1.17 3.64Zm1.51-.203h7.254l1.268-3.944.01-.023a2.536 2.536 0 0 0-.295-2.409l-3.86-4.686v4.514a2.418 2.418 0 1 1-1.5 0V3.188L5.39 7.874a2.536 2.536 0 0 0-.294 2.41l.009.022 1.268 3.944ZM10 10.916a.917.917 0 1 0 0-1.833.917.917 0 0 0 0 1.833Z" clip-rule="evenodd"/>
                    </svg>
                    <span class="text-lg font-semibold">Blog</span> 
                </div>
                <svg class="chevron w-6 h-6 text-orange-600" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                </svg>
            </div>
            <div class="accordion-content flex flex-col mt-4 text-sm font-medium">
                <a href="#" class="py-3">Lead generation</a>
                <a href="#" class="py-3">Sales</a>
                <a href="#" class="py-3">Outreach</a>
                <a href="#" class="py-3">B2B marketing</a>
                <a href="#" class="py-3 flex items-center gap-x-1">
                    <span>See all</span>
                    <svg class="w-4 h-4" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M4.5 12h15m0 0l-6.75-6.75M19.5 12l-6.75 6.75" />
                    </svg>
                </a>
            </div>
        </div>
        <!-- accordion-item -->
        <div class="accordion-item py-4">
            <div class="accordion-header w-full text-xl flex items-center justify-between">
                <div class="flex items-center gap-x-2">
                    
                    <svg class="w-6 h-6" width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M17.5 12.25V7.75C17.5 4 16 2.5 12.25 2.5H7.75C4 2.5 2.5 4 2.5 7.75V12.25C2.5 16 4 17.5 7.75 17.5H12.25C16 17.5 17.5 16 17.5 12.25Z" stroke="#FF5E00" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                        <path d="M2.89014 6.33203H17.1101" stroke="#FF5E00" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                        <path d="M7.39014 2.58203V6.22703" stroke="#FF5E00" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                        <path d="M12.6099 2.58203V5.88953" stroke="#FF5E00" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                        <path d="M8.3125 11.8371V10.9371C8.3125 9.7821 9.13 9.3096 10.1275 9.8871L10.9075 10.3371L11.6875 10.7871C12.685 11.3646 12.685 12.3096 11.6875 12.8871L10.9075 13.3371L10.1275 13.7871C9.13 14.3646 8.3125 13.8921 8.3125 12.7371V11.8371V11.8371Z" stroke="#FF5E00" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
                    </svg>

                    
                    <span class="text-lg font-semibold">Knowledge</span> 
                </div>
                <svg class="chevron w-6 h-6 text-orange-600" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                </svg>
            </div>
            <div class="accordion-content flex flex-col mt-4 text-sm font-medium">
                <a href="#" class="py-3">Growth podcast</a>
                <a href="#" class="py-3">Webinars</a>
                <a href="#" class="py-3">Resources library</a>
            </div>
        </div>
    </div>

    <!-- banner -->
    <div class="mt-4 min-h-[17.4rem] rounded-2xl overflow-hidden flex relative bg-[#D6DDF5]">
        <img class="z-0 absolute w-[256px] h-[256px] -top-[91px] -left-[72px]" src="/assets/images/header/resources-banner-background-element-1.webp">
        <img class="z-0 absolute -top-[50px] -right-[40px]" src="/assets/images/header/resources-banner-background-element-2.webp">
        <img class="z-0 absolute w-[119px] h-[119px] bottom-[61px] right-12 " src="/assets/images/header/resources-banner-background-element-3.webp">
        <div class="z-10  flex flex-col gap-y-6 px-4 py-8">
            <div class="flex flex-col gap-y-3">
                <h1 class="text-[1.75rem] font-bold leading-10">
                    <div>Join the <span class="text-blue-500">Belkins</span> </div>
                    <div class="text-blue-500">community</div>
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