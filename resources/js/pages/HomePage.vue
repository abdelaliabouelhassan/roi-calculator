<template>
    <div class="bg-gray-100">
        <FirstSection />
       <FifthSection />
        <!-- <p class="">This is my HOME PAGE component content.</p> -->
    </div>
</template>
<script>
import FirstSection  from '../components/partials/home/FirstSection.vue'
import FifthSection  from '../components/partials/home/FifthSection.vue'
export default {
    components:{
        FirstSection,FifthSection
    }
}
</script>
