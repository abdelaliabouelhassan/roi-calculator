<template>
    <section class="flex flex-col items-center gap-y-6 container mx-auto xl:max-w-[67.25rem] px-4 py-12 lg:pt-16 lg:pb-12 lg:flex-row lg:justify-between lg:gap-x-24 
                    xl:pt-20 xl:pb-16">
        
        <div class="flex flex-col gap-y-6 w-full ">
            <h1 class="text-2xl font-bold lg:text-[2rem]">How it works</h1>
            <p class="lg:text-lg">Our ROI calculator is designed to help you determine the potential return on investment you can achieve by working with Prospecta.</p>
        </div>

        <div class="z-10 relative rounded-2xl border border-white flex flex-col w-full max-w-[496px]">
            <!-- ball -->
            <div class="animate-[levitation-1_30s_infinite] z-0 absolute -top-[40px] right-[56px] w-14 h-14 lg:w-20 lg:h-20 bg-bright-purple-gradient .shadow-bullet-purple rounded-full">
            </div>
            <div class="z-10 h-full rounded-t-2xl overflow-hidden  flex flex-col items-center justify-between gap-y-2 text-purple-500 py-8 px-16 bg-white bg-opacity-70 backdrop-blur-md">
                <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M11.4272 20.3601L20.1472 11.6401" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                    <path d="M11.9735 13.8269C12.8793 13.8269 13.6135 13.0926 13.6135 12.1869C13.6135 11.2811 12.8793 10.5469 11.9735 10.5469C11.0678 10.5469 10.3335 11.2811 10.3335 12.1869C10.3335 13.0926 11.0678 13.8269 11.9735 13.8269Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                    <path d="M20.6932 21.4533C21.5989 21.4533 22.3332 20.7191 22.3332 19.8133C22.3332 18.9076 21.5989 18.1733 20.6932 18.1733C19.7874 18.1733 19.0532 18.9076 19.0532 19.8133C19.0532 20.7191 19.7874 21.4533 20.6932 21.4533Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                    <path d="M15.9998 29.3332C23.3636 29.3332 29.3332 23.3636 29.3332 15.9998C29.3332 8.63604 23.3636 2.6665 15.9998 2.6665C8.63604 2.6665 2.6665 8.63604 2.6665 15.9998C2.6665 23.3636 8.63604 29.3332 15.9998 29.3332Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
                <div class="text-sm font-semibold lg:text-xl">Return on investment (ROI)</div>
            </div>    
            <div class="z-10 h-full rounded-b-2xl overflow-hidden w-full bg-[#F7F7F7] ">
                <div class="flex items-center justify-center gap-x-4 px-11 py-[22px] lg:py-8 lg:px-16">
                    <div class="flex flex-col items-center divide-y text-[11px] lg:text-base">
                        <div class="flex items-center gap-x-1 text-[#292929] pb-1.5">
                            <svg width="20" height="21" viewBox="0 0 20 21" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M7.9165 11.959C7.9165 12.7673 8.54152 13.4173 9.30818 13.4173H10.8748C11.5415 13.4173 12.0832 12.8507 12.0832 12.1423C12.0832 11.384 11.7498 11.109 11.2582 10.934L8.74984 10.059C8.25817 9.88401 7.92485 9.61735 7.92485 8.85068C7.92485 8.15068 8.4665 7.57568 9.13316 7.57568H10.6998C11.4665 7.57568 12.0915 8.22568 12.0915 9.03402" stroke="#8A8A8A" stroke-width="1.25" stroke-linecap="round" stroke-linejoin="round"/>
                                <path d="M10 6.75V14.25" stroke="#8A8A8A" stroke-width="1.25" stroke-linecap="round" stroke-linejoin="round"/>
                                <path d="M18.3332 10.5003C18.3332 15.1003 14.5998 18.8337 9.99984 18.8337C5.39984 18.8337 1.6665 15.1003 1.6665 10.5003C1.6665 5.90033 5.39984 2.16699 9.99984 2.16699" stroke="#8A8A8A" stroke-width="1.25" stroke-linecap="round" stroke-linejoin="round"/>
                                <path d="M14.1665 3V6.33333H17.4998" stroke="#8A8A8A" stroke-width="1.25" stroke-linecap="round" stroke-linejoin="round"/>
                                <path d="M18.3332 2.16699L14.1665 6.33366" stroke="#8A8A8A" stroke-width="1.25" stroke-linecap="round" stroke-linejoin="round"/>
                            </svg>
                            <div class="font-medium">Net profit</div>
                        </div>
                        <div class="flex items-center gap-x-1 text-[#292929] pt-1.5">
                            <svg width="20" height="21" viewBox="0 0 20 21" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M14.7835 19.4585H10.2169C9.87519 19.4585 9.59185 19.1752 9.59185 18.8335C9.59185 18.4918 9.87519 18.2085 10.2169 18.2085H14.7835C16.1669 18.2085 17.2919 17.0835 17.2919 15.7002V15.3335H16.3335C15.0752 15.3335 14.0085 14.4002 13.9085 13.2002C13.8419 12.5085 14.0919 11.8335 14.5919 11.3418C15.0169 10.9085 15.6002 10.6668 16.2252 10.6668H17.2835V10.0918C17.2835 8.7085 16.1585 7.5835 14.7752 7.5835H5.20852C3.82519 7.5835 2.7002 8.7085 2.7002 10.0918V11.5335C2.7002 11.8752 2.41686 12.1585 2.0752 12.1585C1.73353 12.1585 1.4502 11.8752 1.4502 11.5335V10.0918C1.4502 8.01684 3.13352 6.3335 5.20852 6.3335H14.7752C16.8502 6.3335 18.5335 8.01684 18.5335 10.0918V11.2918C18.5335 11.6335 18.2502 11.9168 17.9085 11.9168H16.2252C15.9335 11.9168 15.6669 12.0252 15.4752 12.2252C15.2335 12.4585 15.1169 12.7752 15.1502 13.0918C15.2002 13.6418 15.7252 14.0835 16.3252 14.0835H17.9085C18.2502 14.0835 18.5335 14.3668 18.5335 14.7085V15.7002C18.5419 17.7752 16.8585 19.4585 14.7835 19.4585Z" fill="#8A8A8A"/>
                                <path d="M2.08325 11.4665C1.74159 11.4665 1.45825 11.1832 1.45825 10.8415V7.03322C1.45825 5.79155 2.24159 4.66651 3.39992 4.22484L10.0166 1.72484C10.6999 1.46651 11.4583 1.55822 12.0499 1.97488C12.6499 2.39155 12.9999 3.06654 12.9999 3.79154V6.9582C12.9999 7.29987 12.7166 7.5832 12.3749 7.5832C12.0333 7.5832 11.7499 7.29987 11.7499 6.9582V3.79154C11.7499 3.47488 11.5999 3.1832 11.3333 2.99987C11.0666 2.81653 10.7499 2.77486 10.4499 2.89153L3.83326 5.39153C3.15826 5.64986 2.69992 6.30822 2.69992 7.03322V10.8415C2.70826 11.1915 2.42492 11.4665 2.08325 11.4665Z" fill="#8A8A8A"/>
                                <path d="M16.3333 15.3336C15.075 15.3336 14.0083 14.4003 13.9083 13.2003C13.8416 12.5086 14.0916 11.8337 14.5916 11.342C15.0166 10.9087 15.6 10.667 16.225 10.667H17.9583C18.7833 10.692 19.4166 11.342 19.4166 12.142V13.8587C19.4166 14.6587 18.7833 15.3086 17.9833 15.3336H16.3333ZM17.9416 11.917H16.2333C15.9416 11.917 15.675 12.0253 15.4833 12.2253C15.2416 12.4587 15.125 12.7753 15.1583 13.092C15.2083 13.642 15.7333 14.0836 16.3333 14.0836H17.9666C18.075 14.0836 18.175 13.9837 18.175 13.8587V12.142C18.175 12.017 18.075 11.9253 17.9416 11.917Z" fill="#8A8A8A"/>
                                <path d="M11.6666 11.125H5.83325C5.49159 11.125 5.20825 10.8417 5.20825 10.5C5.20825 10.1583 5.49159 9.875 5.83325 9.875H11.6666C12.0083 9.875 12.2916 10.1583 12.2916 10.5C12.2916 10.8417 12.0083 11.125 11.6666 11.125Z" fill="#8A8A8A"/>
                                <path d="M7.91667 16.9083C7.575 16.9083 7.29167 16.625 7.29167 16.2833V15.2166C7.29167 15.0333 7.14166 14.875 6.95 14.875H2.5C2.15833 14.875 1.875 14.5917 1.875 14.25C1.875 13.9083 2.15833 13.625 2.5 13.625H6.95C7.825 13.625 8.54167 14.3416 8.54167 15.2166V16.2833C8.54167 16.625 8.25833 16.9083 7.91667 16.9083Z" fill="#8A8A8A"/>
                                <path d="M3.51654 15.8916C3.3582 15.8916 3.19987 15.8333 3.07487 15.7083L2.0582 14.6916C1.81654 14.45 1.81654 14.0499 2.0582 13.8082L3.07487 12.7916C3.31654 12.5499 3.71654 12.5499 3.9582 12.7916C4.19987 13.0333 4.19987 13.4333 3.9582 13.6749L3.3832 14.2499L3.9582 14.8249C4.19987 15.0666 4.19987 15.4666 3.9582 15.7083C3.8332 15.8333 3.67487 15.8916 3.51654 15.8916Z" fill="#8A8A8A"/>
                                <path d="M7.91667 19.275H3.46667C2.59167 19.275 1.875 18.5583 1.875 17.6833V16.6167C1.875 16.275 2.15833 15.9917 2.5 15.9917C2.84167 15.9917 3.125 16.275 3.125 16.6167V17.6833C3.125 17.8667 3.275 18.025 3.46667 18.025H7.91667C8.25833 18.025 8.54167 18.3084 8.54167 18.65C8.54167 18.9917 8.25833 19.275 7.91667 19.275Z" fill="#8A8A8A"/>
                                <path d="M6.90026 20.2915C6.74193 20.2915 6.58359 20.2332 6.45859 20.1082C6.21693 19.8665 6.21693 19.4665 6.45859 19.2248L7.0336 18.6498L6.45859 18.0748C6.21693 17.8332 6.21693 17.4332 6.45859 17.1915C6.70026 16.9498 7.10026 16.9498 7.34193 17.1915L8.35859 18.2081C8.60026 18.4498 8.60026 18.8498 8.35859 19.0915L7.34193 20.1082C7.22526 20.2332 7.05859 20.2915 6.90026 20.2915Z" fill="#8A8A8A"/>
                            </svg>
                            <div class="font-medium">Cost of investment</div>
                        </div>
                    </div>
                    <div class="roi-calculator-formula w-20 h-[45px] lg:w-[115px] lg:h-16  flex items-center justify-center text-[13px] lg:text-lg font-medium rounded-2xl">x100</div>
                </div>
            </div>
                
            
        </div>
    </section>
</template>
<style scoped>
.bg-bright-purple-gradient {
    background-image: radial-gradient(72.33% 86.91% at 26.44% 13.09%,#ff98f5 12.69%,#a855f7 64.54%,#ff3ff2 100%);
}
.shadow-bullet-purple {
    box-shadow: 0 0 #0000,0 0 #0000,12px 24px 48px 0px rgba(169, 85, 247, 0.322);
}





.roi-calculator-formula {
    background: linear-gradient(135.54deg,hsla(17,13%,90%,.4) -10.59%,hsla(0,0%,96%,.4) 62.79%);
    box-shadow: 0.830588px 0.830588px #ffffffe6, inset 5.30756px 4.24605px 13.81px #e4ddd833, inset -5.30756px -5.30756px 8.49209px #fff3;
}

</style>