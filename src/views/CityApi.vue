<script>
export default {
    data() {
        return {
            scroch: '',
            arr: [],
            showarr: [],
        }
    },

    mounted() {
        fetch('https://gist.githubusercontent.com/Miserlou/c5cd8364bf9b2420bb29/raw/2bf258763cdddd704f8ffd3ea9a3e81d25e2c6f6/cities.json')
            .then(response => {
                return response.json();
            })
            .then(data => {
                //抓取數據
                this.arr = data;
                this.showarr = data;
            })
    },

    computed: {

        // return this.arr.filter((item)=>{
        //     if(this.showarr === 'city'){
        //         return this.showarr;
        //     }
        // })
    },

    methods: {
        // 資料搜尋
        citys(e) {
            // 先找到INPUT的值
            console.log(e.target.value)
            // 從完整資料中去過濾所打的內容(過濾城市名稱)
            let longWords = this.arr.filter((item) => item.city.includes(e.target.value));
            // 把過濾的內容塞到顯示的資料欄位上
            this.showarr =longWords; !
            console.log(longWords)
        },
    },
};

</script>
<template>
    <div class="body w-screen h-full flex items-center flex-col pt-20 bg-amber-200">
        <div class="box">
            <!-- {{ this.scroch }} -->
            <input type="text" @change="(e) => citys(e)" class="add-text w-[40rem] h-[10rem] rounded-lg mb-10 text-5xl">
        </div>
        <div class="w-[40rem] h-full flex justify-around" v-for="(item, index) in showarr" :key="item.rank">
            <div class="w-[250px] h[20px] mb-3 text-2xl  rounded-lg border-2 border-white bg-blue-300">{{ item.city }}</div>
            <div class="w-[150px] h[20px] mb-3 text-2xl  rounded-lg border-2 border-white bg-blue-300">{{ item.population }}</div>
             
        </div>
    </div>
</template>
<style scoped></style>