<template>
    <div class="mt-12">
        <div class="flex flex-col divide-y px-8 py-2" >
            <button @click="$emit('changeComponent','SmallScreenWhatWeDo')" class="w-full text-xl flex items-center justify-between py-4">
                <span class="text-lg font-semibold">What we do</span> 
                <svg class="w-6 h-6 text-orange-600" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                </svg>
            </button>
            <button @click="$emit('changeComponent','SmallScreenCustomerSuccess')" class="w-full text-xl flex items-center justify-between py-4">
                <span class="text-lg font-semibold">Customer success</span> 
                <svg class="w-6 h-6 text-orange-600" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                </svg>
            </button>
            <button @click="$emit('changeComponent','SmallScreenRecources')" class="w-full text-xl flex items-center justify-between py-4">
                <span class="text-lg font-semibold">Recources</span> 
                <svg class="w-6 h-6 text-orange-600" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                </svg>
            </button>
            <button @click="$emit('changeComponent','SmallScreenCompany')" class="w-full text-xl flex items-center justify-between py-4">
                <span class="text-lg font-semibold">Company</span> 
                <svg class="w-6 h-6 text-orange-600" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8.25 4.5l7.5 7.5-7.5 7.5" />
                </svg>
            </button>
            <a href="#" class="text-xl flex items-center justify-between py-4">
                <span class="text-lg font-semibold">Pricing</span> 
            </a>
            <a href="#" class="text-xl flex items-center justify-between py-4">
                <span class="text-lg font-semibold">Contact Us</span> 
            </a>
        </div>
        
    </div>
</template>