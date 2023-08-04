<template>
    <div class="bg-gray-100">
        <FirstSection />
        <SecondSection />
        <!-- <ThirdSection />
        <FourthSection />
        <FifthSection />
        <SixthSection />-->
        <SeventhSection /> 
        <!-- <p class="">This is my HOME PAGE component content.</p> -->
    </div>
</template>
<script>
import FirstSection  from '../components/partials/home/FirstSection.vue'
import SecondSection  from '../components/partials/home/SecondSection.vue'
import ThirdSection  from '../components/partials/home/ThirdSection.vue'
import FourthSection  from '../components/partials/home/FourthSection.vue'
import FifthSection  from '../components/partials/home/FifthSection.vue'
import SixthSection  from '../components/partials/home/SixthSection.vue'
import SeventhSection  from '../components/partials/home/SeventhSection.vue'
export default {
    components:{
        FirstSection,SecondSection,ThirdSection,FourthSection,FifthSection,SixthSection,SeventhSection
    }
}
</script>
