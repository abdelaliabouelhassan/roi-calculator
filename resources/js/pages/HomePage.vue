<template>
    <div class="bg-gray-100">
        <FirstSection />
        <SecondSection />
        <FifthSection />
        <SixthSection />
        <!-- <p class="">This is my HOME PAGE component content.</p> -->
    </div>
</template>
<script>
import FirstSection  from '../components/partials/home/FirstSection.vue'
import SecondSection  from '../components/partials/home/SecondSection.vue'
import FifthSection  from '../components/partials/home/FifthSection.vue'
import SixthSection  from '../components/partials/home/SixthSection.vue'
export default {
    components:{
        FirstSection,SecondSection,FifthSection,SixthSection
    }
}
</script>
