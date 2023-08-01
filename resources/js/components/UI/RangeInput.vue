<template>
    <input class="range-input" type="range" v-model="value" :min="min" :max="max" :step="step">
</template>
<script>
export default {
    emits: ['update:modelValue'],
    props:{
        modelValue:{
            required:true
        },
        min:{
            type:Number,
            required:true
        },
        max:{
            type:Number,
            required:true
        },
        step:{
            type:Number,
            default:1
        }
    },
    data() {
        return {
            value:null
        }
    },
    computed:{
        inputBackground(){
            return `linear-gradient(to right, rgb(168 85 247) ${(this.value * 100 / (this.max - this.min)) - (this.min * 100 / (this.max - this.min)) }%, rgb(235, 235, 235) ${(this.value * 100 / (this.max - this.min)) - (this.min * 100 / (this.max - this.min)) }%, rgb(235, 235, 235) 100%) `
        }
    },
    watch:{
        
        value(val){
            this.$emit('update:modelValue', val)
        },
        modelValue:{
            handler(val){
                this.value = val
            },
            immediate:true
        }
    }
    
}
</script>

<style scoped>
.range-input{
    -webkit-appearance: none;
    background:  v-bind('inputBackground') ;
    border: none;
    border-radius: 3px 3px 0 0;
    outline: none;
    color: rgb(168 85 247);

}
.range-input::-webkit-slider-runnable-track {
    height: 3.5px;
    -webkit-appearance: none;
    margin-top: -1px;

}
    
.range-input::-webkit-slider-thumb {
    width: 14px;
    -webkit-appearance: none;
    height: 14px;
    cursor: pointer;
    border-radius: 50px;
    background: rgb(168 85 247);
    margin-top: -5px;
}
.range-input::-webkit-slider-thumb:active {
    outline: rgba(169, 85, 247, 0.3) 3px solid;
}
</style>