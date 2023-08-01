<template>
    <header class="z-50 fixed top-0 left-0 w-full bg-white h-[4.5rem]">
        <div class="flex flex-col ">
            <nav class="z-40 w-full flex justify-between py-4 px-4 md:justify-start md:gap-x-16">
                <!-- <img class="w-[90px]" src="/images/logos/logo-black.svg" alt="" srcset=""> -->
                <div class="flex items-center">

                    <button @click="showMenu = !showMenu" class="w-6 h-6 flex flex-col justify-between items-center xl:hidden mr-6" aria-label="toggle menu">
                        <span class="w-full h-[3px] bg-black rounded-full origin-right transition-all duration-200 ease" :class="{'-rotate-45 translate-y-[2px]':showMenu}"></span>
                        <span class="w-full h-[3px] bg-black rounded-full transition-opacity duration-200 ease" :class="{'opacity-0':showMenu}"></span>
                        <span class="w-full h-[3px] bg-black rounded-full origin-right transition-all duration-200 ease" :class="{'rotate-45 -translate-y-[2px]':showMenu}"></span>
                    </button>
                    <div class="w-[90px] h-[32px] bg-red-300">

                    </div>

                    <!-- xl screen menu -->
                    <div class="hidden xl:flex gap-x-8 h-fit">
                        <a href="#" class="text-xl">What we do</a>
                        <a href="#" class="text-xl">Customer success</a>
                        <a href="#" class="text-xl">Recources</a>
                        <a href="#" class="text-xl">Company</a>
                        <a href="#" class="text-xl">Pricing</a>
                    </div>
                </div>
                <div>
                    <button class="py-2 px-4 bg-orange-600 text-white font-semibold rounded-md text-sm">
                        book a call
                    </button>
                </div>


            </nav>
            <!-- small screen menu content-->
            <div class="xl:hidden h-[calc(100vh-4.5rem)] px-4 w-full flex flex-col transition-all duration-500 ease-in-out overflow-y-auto "
                :class="{'hidden':!showMenu}">
                <component :is='currentSmallMenuComponent' @changeComponent="changeComponent"></component>
                <div class="py-8 mt-4 flex justify-between items-center text-sm font-semibold">
                    <div class="flex items-center gap-x-2">
                        <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M5.00008 6.66667L8.15108 8.76733C8.71091 9.14055 10.0001 10 10.0001 10C10.0001 10 11.2892 9.14055 11.8491 8.76733L15.0001 6.66667M5.00008 17.5H15.0001C16.841 17.5 18.3334 16.0076 18.3334 14.1667V5.83333C18.3334 3.99238 16.841 2.5 15.0001 2.5H5.00008C3.15913 2.5 1.66675 3.99238 1.66675 5.83333V14.1667C1.66675 16.0076 3.15913 17.5 5.00008 17.5Z" stroke="#B8B8B8" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                        </svg>
                        <span>sales@belkins.io</span>
                    </div>
                    <div class="flex items-center gap-x-2">
                        <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M14.7916 12.4962C14.2807 11.9009 13.5549 11.8214 12.9084 12.2901C12.4157 12.6462 11.923 13.0024 11.4387 13.3684C11.3055 13.4697 11.2031 13.4808 11.0656 13.39C10.7994 13.2138 10.5104 13.0662 10.2554 12.8779C9.07409 11.9953 8.12417 10.9195 7.31326 9.73423C6.912 9.14649 6.56264 8.52877 6.35564 7.85085C6.31552 7.71273 6.33091 7.62972 6.46295 7.53719C6.95453 7.18981 7.43774 6.83259 7.92096 6.47537C8.59511 5.97858 8.67915 5.31914 8.14424 4.68557C7.84359 4.32726 7.53821 3.96844 7.23226 3.61401C6.91851 3.24536 6.6095 2.87722 6.291 2.50804C5.77476 1.91664 5.05429 1.83333 4.40304 2.30143C3.91034 2.65761 3.42544 3.02801 2.92912 3.37488C2.46462 3.69848 2.19401 4.12354 2.08409 4.64642C1.90899 5.49203 2.02885 6.32535 2.24639 7.14706C2.69372 8.84532 3.50137 10.3958 4.53231 11.8548C5.92605 13.826 7.69054 15.4545 9.8322 16.7275C10.7933 17.3007 11.811 17.7687 12.9564 17.952C13.7436 18.0783 14.4597 17.9694 15.0828 17.4581C15.5121 17.1084 15.9797 16.7985 16.4305 16.4689C17.0941 15.9799 17.1845 15.3078 16.6663 14.6939C16.0388 13.9565 15.4149 13.2285 14.7916 12.4962Z" stroke="#B8B8B8" stroke-width="1.5"/>
                        </svg>
                        <span>+1 302-803-5506</span>
                    </div>
                </div>
            </div>




        </div>
    </header>
</template>

<script > 
import SmallScreenMenu from './includes/SmallScreenMenu.vue'
import SmallScreenWhatWeDo from './includes/SmallScreenWhatWeDo.vue'
import SmallScreenCompany from './includes/SmallScreenCompany.vue'
import SmallScreenCustomerSuccess from './includes/SmallScreenCustomerSuccess.vue'
import SmallScreenRecources from './includes/SmallScreenRecources.vue'
export default {
    components:{
        SmallScreenMenu, SmallScreenWhatWeDo,SmallScreenCompany ,SmallScreenCustomerSuccess,SmallScreenRecources
    },
    data(){
        return{
            showMenu: false,
            currentSmallMenuComponent:'SmallScreenMenu'
        }
    },
    methods: {
        changeComponent(component){
            this.currentSmallMenuComponent = component
        }
    },
}
</script>

