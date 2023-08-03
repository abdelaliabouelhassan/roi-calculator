<template>
    <section class="flex relative text-white lg:h-[436px] w-full h-[484px] items-center justify-center">
        <img class="w-full h-full object-cover absolute top-0 left-0" src="/assets/images/home/seventh-section/bg-grow-cta.webp" alt="" srcset="">
        <div class="z-10 h-fit flex flex-col gap-y-6 w-full py-8 px-6 rounded-2xl border border-white/10 backdrop-blur-lg
             cta-grow-bg mx-8 lg:w-[800px] lg:mx-auto lg:p-12 lg:flex-row lg:items-center lg:justify-between lg:gap-x-16
             xl:w-[1042px]">
             <div class="flex flex-col gap-y-6 ">
                <h1 class="text-4xl font-bold w-full max-w-[248px] lg:max-w-none xl:text-5xl leading-[44px] lg:leading-[48px]">Want to grow revenue?</h1>
                <p class="text-lg  w-full max-w-[248px]  lg:max-w-none">Let's elevate your lead gen results and book you more qualified appointments.</p>
             </div>
            <button class="bg-purple-500 rounded-lg  text-white font-bold text-lg p-4 pl-6 flex items-center justify-between gap-x-6 lg:w-fit lg:shrink-0 w-full hover:bg-purple-500/70">
                <span>Get started</span>
                <svg width="24" height="24" fill="none" xmlns="http://www.w3.org/2000/svg" class="rotate-0">
                    <path d="m10 18 6-6-6-6" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
                </svg>
            </button>
        </div>
    </section>
</template>

<style scoped>
.cta-grow-bg {
    background: linear-gradient(0deg,hsla(0,0%,100%,.1),hsla(0,0%,100%,.1)),rgba(0,0,0,.2);
}
</style>