<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-md-8">
                <div class="card space-y-10">
                    <div class="  text-gray-600 font-bold line-through">Example Component</div>

                    <div class=" text-blue-500 text-5xl">
                        I'm an example component.
                    </div>
                    <div class=" text-yellow-300 text-7xl ease-linear">
                        use this logo for this project
                    </div>

                    <div class="">
                        <img src="/assets/logo.svg" alt="">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        mounted() {
            console.log('Component mounted.')
            alert('Indeed,')
        }
    }
</script>
