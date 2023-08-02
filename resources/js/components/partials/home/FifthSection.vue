<template>
    <section>
         <TestimonialCard>
            <template #img>
                <img src="/assets/images/json-wong.webp" alt="" srcset="">
            </template>
            <template #name>
                Jason Wong
            </template>
            <template #role>
                CEO at Omnicharge
            </template>
            <template #testimony>
                The work of the Belkins team was very productive. We were especially impressed by the deep research - it seemed that Belkins experts started speaking our brand’s language after delving into our style guidelines and investigating them for a while.
            </template>
        </TestimonialCard>
    </section>
</template>
<script>
import TestimonialCard  from '../../UI/TestimonialCard.vue'
export default {
    components:{
        TestimonialCard
    }
}
</script>