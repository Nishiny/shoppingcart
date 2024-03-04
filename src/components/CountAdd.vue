<script>
export default {
    //傳進來的值 跟data是一樣的東西
    props:{
        buttonText:{
            type: String,
        },
        buttonNumber:{
            type: Number,
        },
    },
    emits:['submit'],
    data() {
        return {
            count: 1,
        };
    },
    methods:{
        sumNumber() {
            // console.log(12);
            this.$emit('submit', this.count *= this.buttonNumber);
        }
    },
};

</script>

<template>
    {{ count }}
    <button class="text-3xl bg-red-300" @click="sumNumber()">{{ buttonText }}</button>
</template>