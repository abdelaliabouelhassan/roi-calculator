<template>
    <div class="testimonial-card relative flex transition-opacity duration-200 ease-in-out">
        <svg class="absolute -top-[40px] right-6 z-0 quotes-img opacity-100 transition-opacity duration-600 ease-in-out text-purple-500" width="180" height="104" viewBox="0 0 180 104" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path fill-rule="evenodd" clip-rule="evenodd"
                d="M139.056 104C116.441 104 98.1064 86.3681 98.1064 64.6137C98.1064 33.7394 120.156 16.1259 144.174 0.534478C146.904 -1.23424 150.294 1.72284 148.723 4.50949C144.955 11.2113 142.364 18.1065 141.727 25.3104C163.097 26.6369 180 43.7253 180 64.6137C180 86.3681 161.666 104 139.056 104Z"
                fill="currentColor"/>
            <path fill-rule="evenodd" clip-rule="evenodd"
                d="M40.9445 104C18.3344 104 0.00012275 86.3681 0.00012275 64.6137C0.00012275 33.7394 22.0453 16.1259 46.0632 0.534478C48.7925 -1.23424 52.1826 1.72284 50.6168 4.50949C46.8484 11.2113 44.2532 18.1065 43.6211 25.3104C64.9863 26.6369 81.8937 43.7253 81.8937 64.6137C81.8937 86.3681 63.5594 104 40.9445 104Z"
                fill="currentColor"/>
            <defs>
                <linearGradient id="paint0_linear_3176:2870" x1="98.1064" y1="104" x2="182.975" y2="101.513"
                                gradientUnits="userSpaceOnUse">
                    <stop stop-color="currentColor"/>
                    <stop offset="1" stop-color="currentColor"/>
                </linearGradient>
                <linearGradient id="paint1_linear_3176:2870" x1="0.00012268" y1="104" x2="84.8689" y2="101.513"
                                gradientUnits="userSpaceOnUse">
                    <stop stop-color="currentColor"/>
                    <stop offset="1" stop-color="currentColor"/>
                </linearGradient>
            </defs>
        </svg>
        <div class="content-wrapper h-full flex flex-col gap-y-5 z-10 p-8  rounded-2xl border backdrop-blur-md bg-opacity-60 border-white bg-white
                    ">
            <div class="flex items-center gap-x-4">
                <!-- img -->
                <div class="max-w-[80px] max-h-[80px]">
                    <slot name="img" />
                </div>
                <div class="flex flex-col gap-y-1">
                    <!-- stars -->
                    <div class="flex items-center gap-x-1">
                        <svg class="w-4 h-4" width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M19.2803 8.27282C19.5471 8.0379 19.3978 7.5978 19.0432 7.57359L12.9877 7.16001C12.8323 7.1494 12.6972 7.04953 12.6414 6.90407L10.3695 0.974811C10.2383 0.632306 9.75373 0.632306 9.6225 0.974811L7.35057 6.90409C7.29484 7.04954 7.15974 7.14941 7.00434 7.16003L0.955737 7.57359C0.601299 7.59782 0.451991 8.03762 0.71842 8.27263L5.38619 12.3899C5.4978 12.4884 5.54552 12.6407 5.51007 12.7852L3.983 19.012C3.89645 19.3649 4.2873 19.6411 4.59104 19.4416L9.77646 16.0367C9.90975 15.9492 10.0823 15.9492 10.2156 16.0367L15.401 19.4416C15.7048 19.6411 16.0956 19.3649 16.0091 19.012L14.482 12.7854C14.4466 12.6408 14.4944 12.4884 14.6061 12.3899L19.2803 8.27282Z" fill="#FF5E00"/>
                        </svg>
                        <svg class="w-4 h-4" width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M19.2803 8.27282C19.5471 8.0379 19.3978 7.5978 19.0432 7.57359L12.9877 7.16001C12.8323 7.1494 12.6972 7.04953 12.6414 6.90407L10.3695 0.974811C10.2383 0.632306 9.75373 0.632306 9.6225 0.974811L7.35057 6.90409C7.29484 7.04954 7.15974 7.14941 7.00434 7.16003L0.955737 7.57359C0.601299 7.59782 0.451991 8.03762 0.71842 8.27263L5.38619 12.3899C5.4978 12.4884 5.54552 12.6407 5.51007 12.7852L3.983 19.012C3.89645 19.3649 4.2873 19.6411 4.59104 19.4416L9.77646 16.0367C9.90975 15.9492 10.0823 15.9492 10.2156 16.0367L15.401 19.4416C15.7048 19.6411 16.0956 19.3649 16.0091 19.012L14.482 12.7854C14.4466 12.6408 14.4944 12.4884 14.6061 12.3899L19.2803 8.27282Z" fill="#FF5E00"/>
                        </svg>
                        <svg class="w-4 h-4" width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M19.2803 8.27282C19.5471 8.0379 19.3978 7.5978 19.0432 7.57359L12.9877 7.16001C12.8323 7.1494 12.6972 7.04953 12.6414 6.90407L10.3695 0.974811C10.2383 0.632306 9.75373 0.632306 9.6225 0.974811L7.35057 6.90409C7.29484 7.04954 7.15974 7.14941 7.00434 7.16003L0.955737 7.57359C0.601299 7.59782 0.451991 8.03762 0.71842 8.27263L5.38619 12.3899C5.4978 12.4884 5.54552 12.6407 5.51007 12.7852L3.983 19.012C3.89645 19.3649 4.2873 19.6411 4.59104 19.4416L9.77646 16.0367C9.90975 15.9492 10.0823 15.9492 10.2156 16.0367L15.401 19.4416C15.7048 19.6411 16.0956 19.3649 16.0091 19.012L14.482 12.7854C14.4466 12.6408 14.4944 12.4884 14.6061 12.3899L19.2803 8.27282Z" fill="#FF5E00"/>
                        </svg>
                        <svg class="w-4 h-4" width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M19.2803 8.27282C19.5471 8.0379 19.3978 7.5978 19.0432 7.57359L12.9877 7.16001C12.8323 7.1494 12.6972 7.04953 12.6414 6.90407L10.3695 0.974811C10.2383 0.632306 9.75373 0.632306 9.6225 0.974811L7.35057 6.90409C7.29484 7.04954 7.15974 7.14941 7.00434 7.16003L0.955737 7.57359C0.601299 7.59782 0.451991 8.03762 0.71842 8.27263L5.38619 12.3899C5.4978 12.4884 5.54552 12.6407 5.51007 12.7852L3.983 19.012C3.89645 19.3649 4.2873 19.6411 4.59104 19.4416L9.77646 16.0367C9.90975 15.9492 10.0823 15.9492 10.2156 16.0367L15.401 19.4416C15.7048 19.6411 16.0956 19.3649 16.0091 19.012L14.482 12.7854C14.4466 12.6408 14.4944 12.4884 14.6061 12.3899L19.2803 8.27282Z" fill="#FF5E00"/>
                        </svg>
                        <svg class="w-4 h-4" width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M19.2803 8.27282C19.5471 8.0379 19.3978 7.5978 19.0432 7.57359L12.9877 7.16001C12.8323 7.1494 12.6972 7.04953 12.6414 6.90407L10.3695 0.974811C10.2383 0.632306 9.75373 0.632306 9.6225 0.974811L7.35057 6.90409C7.29484 7.04954 7.15974 7.14941 7.00434 7.16003L0.955737 7.57359C0.601299 7.59782 0.451991 8.03762 0.71842 8.27263L5.38619 12.3899C5.4978 12.4884 5.54552 12.6407 5.51007 12.7852L3.983 19.012C3.89645 19.3649 4.2873 19.6411 4.59104 19.4416L9.77646 16.0367C9.90975 15.9492 10.0823 15.9492 10.2156 16.0367L15.401 19.4416C15.7048 19.6411 16.0956 19.3649 16.0091 19.012L14.482 12.7854C14.4466 12.6408 14.4944 12.4884 14.6061 12.3899L19.2803 8.27282Z" fill="#FF5E00"/>
                        </svg>
                        <div class="text-sm font-semibold text-gray-500">5.0</div>
                    </div>
                    <!-- name -->
                    <div class="font-semibold">
                        <slot name="name" />
                    </div>
                    <!-- role -->
                    <div class="text-sm text-gray-500">
                        <slot name="role" />
                    </div>
                </div>
            </div>
            <!-- testimony -->
            <div class="text-sm">
                <slot name="testimony" />
            </div>
        </div>
    </div>
</template>
<style scoped>
@media (min-width: 1000px) {
    li .testimonial-card{
        @apply opacity-40;
    }
    li .testimonial-card .quotes-img{
        @apply opacity-0;
    }
    li.is-active  .testimonial-card, li.is-active  .testimonial-card .quotes-img{
        @apply opacity-100;
    }

    li .testimonial-card .content-wrapper{
        @apply backdrop-blur-0  bg-opacity-100 transition-all duration-700;
    }
    li.is-active .testimonial-card .content-wrapper{
        @apply backdrop-blur-md  bg-opacity-60;
    }
}

</style>