<template>
    <section class="flex flex-col gap-y-8 container mx-auto px-4 py-12 xl:max-w-[67.25rem] xl:px-0 xl:py-24 w-full lg:gap-y-20">
        <div class="w-full h-full flex flex-col lg:items-center gap-y-6 lg:text-center">
            <h1 class="text-[2rem] lg:text-5xl font-bold text-purple-500  md:leading-[56px]  xl:text-[60px]">
                ROI Calculator
            </h1>
            <div class="max-w-[640px] lg:text-lg">
                How much income and ROI can you achieve with Prospecta? Use our calculator to see the real results we can drive for your business.
            </div>
        </div>
        <!-- Roi calculator -->
        <div class="rounded-2xl bg-white flex flex-col lg:flex-row lg:items-center">
            <!-- ranges -->
            <div class="w-full p-4 flex flex-col gap-y-6 lg:p-8">
                <!-- Average # of monthly appointments -->
                <div class="py-3 px-4 relative border rounded-xl flex flex-col gap-y-1 text-sm">
                    <div class="text-[#666666]">
                        Average # of monthly appointments
                    </div> 
                    <div>{{averageMonthlyAppointments}}</div>
                    <RangeInput class="absolute w-[calc(100%-2rem)]  bottom-0" :min="1" :max="100" :step="1" v-model="averageMonthlyAppointments"/>
                </div>
                <!-- Close ratio (after appointment)  -->
                <div class="py-3 px-4 relative border rounded-xl flex flex-col gap-y-1 text-sm">
                    <div class="text-[#666666] flex items-center gap-x-2">
                        <span>
                            Close ratio (after appointment)
                        </span>
                        <!-- info -->
                        <div class="relative group">
                            <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M1.5 8C1.5 7.14641 1.66813 6.30117 1.99478 5.51256C2.32144 4.72394 2.80023 4.00739 3.40381 3.40381C4.00739 2.80023 4.72394 2.32144 5.51256 1.99478C6.30117 1.66813 7.14641 1.5 8 1.5C8.85359 1.5 9.69882 1.66813 10.4874 1.99478C11.2761 2.32144 11.9926 2.80023 12.5962 3.40381C13.1998 4.00739 13.6786 4.72394 14.0052 5.51256C14.3319 6.30117 14.5 7.14641 14.5 8C14.5 9.72391 13.8152 11.3772 12.5962 12.5962C11.3772 13.8152 9.72391 14.5 8 14.5C6.27609 14.5 4.62279 13.8152 3.40381 12.5962C2.18482 11.3772 1.5 9.72391 1.5 8Z" stroke="#A3A3A3"/>
                                <path d="M7.99984 6.83301C8.15455 6.83301 8.30292 6.89447 8.41232 7.00386C8.52171 7.11326 8.58317 7.26163 8.58317 7.41634V10.9163C8.58317 11.0711 8.52171 11.2194 8.41232 11.3288C8.30292 11.4382 8.15455 11.4997 7.99984 11.4997C7.84513 11.4997 7.69675 11.4382 7.58736 11.3288C7.47796 11.2194 7.4165 11.0711 7.4165 10.9163V7.41634C7.4165 7.26163 7.47796 7.11326 7.58736 7.00386C7.69675 6.89447 7.84513 6.83301 7.99984 6.83301Z" fill="#A3A3A3"/>
                                <path d="M7.99981 5.95801C8.11472 5.95801 8.2285 5.93538 8.33466 5.8914C8.44082 5.84743 8.53728 5.78298 8.61853 5.70173C8.69978 5.62048 8.76423 5.52402 8.8082 5.41786C8.85218 5.3117 8.87481 5.19791 8.87481 5.08301C8.87481 4.9681 8.85218 4.85432 8.8082 4.74816C8.76423 4.642 8.69978 4.54554 8.61853 4.46429C8.53728 4.38304 8.44082 4.31859 8.33466 4.27461C8.2285 4.23064 8.11472 4.20801 7.99981 4.20801C7.76805 4.20801 7.54579 4.30007 7.38192 4.46395C7.21804 4.62782 7.12598 4.85009 7.12598 5.08184C7.12598 5.3136 7.21804 5.53586 7.38192 5.69973C7.54579 5.86361 7.76805 5.95567 7.99981 5.95567V5.95801Z" fill="#A3A3A3"/>
                            </svg>
                            <div class="hidden absolute bottom-5 -left-[140px] lg:left-4 bg-white border rounded-xl group-hover:block w-[280px] p-6 text-sm">
                                    To calculate this number, divide the number of sales you made by the number of quotes you sent out.
                            </div>
                        </div>
                        
                    </div> 
                    <div>{{closeRatio}}</div>
                    <RangeInput class="absolute w-[calc(100%-2rem)]  bottom-0" :min="1" :max="100" :step="1" v-model="closeRatio"/>
                </div>
                <!-- Annual contract value (ACV)  -->
                <div class="py-3 px-4 relative border rounded-xl flex flex-col gap-y-1 text-sm">
                    <div class="text-[#666666] flex items-center gap-x-2">
                        <span>
                            Annual contract value (ACV), £
                        </span>
                        <!-- info -->
                        <div class="relative group">
                            <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M1.5 8C1.5 7.14641 1.66813 6.30117 1.99478 5.51256C2.32144 4.72394 2.80023 4.00739 3.40381 3.40381C4.00739 2.80023 4.72394 2.32144 5.51256 1.99478C6.30117 1.66813 7.14641 1.5 8 1.5C8.85359 1.5 9.69882 1.66813 10.4874 1.99478C11.2761 2.32144 11.9926 2.80023 12.5962 3.40381C13.1998 4.00739 13.6786 4.72394 14.0052 5.51256C14.3319 6.30117 14.5 7.14641 14.5 8C14.5 9.72391 13.8152 11.3772 12.5962 12.5962C11.3772 13.8152 9.72391 14.5 8 14.5C6.27609 14.5 4.62279 13.8152 3.40381 12.5962C2.18482 11.3772 1.5 9.72391 1.5 8Z" stroke="#A3A3A3"/>
                                <path d="M7.99984 6.83301C8.15455 6.83301 8.30292 6.89447 8.41232 7.00386C8.52171 7.11326 8.58317 7.26163 8.58317 7.41634V10.9163C8.58317 11.0711 8.52171 11.2194 8.41232 11.3288C8.30292 11.4382 8.15455 11.4997 7.99984 11.4997C7.84513 11.4997 7.69675 11.4382 7.58736 11.3288C7.47796 11.2194 7.4165 11.0711 7.4165 10.9163V7.41634C7.4165 7.26163 7.47796 7.11326 7.58736 7.00386C7.69675 6.89447 7.84513 6.83301 7.99984 6.83301Z" fill="#A3A3A3"/>
                                <path d="M7.99981 5.95801C8.11472 5.95801 8.2285 5.93538 8.33466 5.8914C8.44082 5.84743 8.53728 5.78298 8.61853 5.70173C8.69978 5.62048 8.76423 5.52402 8.8082 5.41786C8.85218 5.3117 8.87481 5.19791 8.87481 5.08301C8.87481 4.9681 8.85218 4.85432 8.8082 4.74816C8.76423 4.642 8.69978 4.54554 8.61853 4.46429C8.53728 4.38304 8.44082 4.31859 8.33466 4.27461C8.2285 4.23064 8.11472 4.20801 7.99981 4.20801C7.76805 4.20801 7.54579 4.30007 7.38192 4.46395C7.21804 4.62782 7.12598 4.85009 7.12598 5.08184C7.12598 5.3136 7.21804 5.53586 7.38192 5.69973C7.54579 5.86361 7.76805 5.95567 7.99981 5.95567V5.95801Z" fill="#A3A3A3"/>
                            </svg>
                            <div class="hidden absolute bottom-5 -left-[140px] lg:left-4 bg-white border rounded-xl group-hover:block w-[280px] p-6 text-sm">
                                The average annual revenue generated from each customer contract, excluding fees.
                            </div>
                        </div>
                        
                    </div> 
                    <div>{{formatNumber(annualContractValue)}}</div>
                    <RangeInput class="absolute w-[calc(100%-2rem)]  bottom-0" :min="25000" :max="5000000" :step="1" v-model="annualContractValue"/>
                </div>
            </div>
            <div class="px-4 py-6 lg:min-w-[400px] lg:w-fit lg:p-8">
                <div class="flex flex-col divide-y">
                    <div class="flex flex-col gap-y-1 pb-5" >
                        <span class="text-sm text-gray-800">Sales per Year</span>
                        <span class="text-2xl lg:text-[2rem] font-bold"> £{{formatNumber(salesPerYear)}}</span>
                    </div>
                    <div class="flex flex-col gap-y-1 py-5" >
                        <span class="text-sm text-gray-800">Investments per Year</span>
                        <span class="text-2xl lg:text-[2rem] font-bold"> £{{formatNumber(investmentPerYear)}}</span>
                    </div>
                    <div class="flex flex-col gap-y-1 py-5" >
                        <span class="text-sm text-gray-800">Return on investment</span>
                        <span class="text-[2rem] lg:text-5xl font-bold text-purple-500"> {{returnOnInvestment < 0 ? 0 :returnOnInvestment.toFixed(0)}}%</span>
                    </div>
                </div>
                <a href="https://calendly.com/joeywalsh/30min" class="bg-purple-500 text-white py-4 px-6 text-lg w-full flex items-center justify-center  font-semibold rounded-lg
                 hover:bg-purple-500/70">
                    Discuss Pricing
                </a>
            </div>
        </div>
        
    </section>
</template>
<script>
import RangeInput from '../../UI/RangeInput.vue'
export default {
    components:{
        RangeInput
    },
    data() {
        return {
            averageMonthlyAppointments:1,
            closeRatio:1,
            annualContractValue:25000
        }
    },
    computed:{
        salesPerYear(){
            // return (this.averageMonthlyAppointments * 12) * this.annualContractValue * this.closeRatio ;
            return (this.averageMonthlyAppointments * 12) * this.annualContractValue * this.closeRatio/100  ;
        },
        investmentPerYear(){
            return (this.averageMonthlyAppointments * 12) * 520;
        },
        returnOnInvestment(){
            return (this.salesPerYear - this.investmentPerYear)*100 / this.investmentPerYear;
        }
    },
    methods:{
        formatNumber(number) {
            return number.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ',');
        }
    }
}
</script>
