<script >
export default {
  data() {
   
  },

  methods:{
  },
}
</script>

<template>
    <div class="w-full p-3 px-5 ">
        <div>
         <h1 class="mb-3 text-3xl font-bold">購物車確認</h1>
        </div>

        <div class="grid-thead">
            <div class="grid-cols-6 grid border-y border-main-deep text-main-deep font-bold py-1 gap-x-3">
                <div class="gird-th text-center"></div>
                <div class="gird-th text-center">商品圖片</div>
                <div class="gird-th">商品名稱</div>
                <div class="gird-th text-center">價錢</div>
                <div class="gird-th opacity-0">操作</div>
            </div>
        </div>

    <div class="grid-thead">
        <div class="grid-cols-6 grid border-y border-main-deep text-main-deep font-bold py-1 gap-x-3">
        <div class="gird-th text-center flex justify-center ">
            <input type="checkbox" class="w-5">
        </div>
        <img src="" alt="">
        <div class="gird-th">手機殼</div>
        <div class="gird-th text-center">$500</div>
        <div class="gird-th">
            <div class="w-[150px] h-[30px] border-[1px] rounded-lg border-black flex justify-around ml-6">
                 <button class="text-3xl mt-[-5px]">-</button>
                 <input class="w-[100px] h-[28px] font-10" type="number">
                 <button class="text-3xl mt-[-5px]">+</button>
            </div>
        </div>  
    </div>
    <div class="flex justify-end flex-wrap">
        <h2 class="text-2xl text-end font-bold w-full">商品數量: 0</h2>
        <h2 class="text-2xl text-end font-bold w-full">商品總金額: $0</h2>
    </div>
    <div class="flex justify-between gap-4">
        <div class="flex justify-center items-center bg-[#8c5046] text-white rounded-md px-4 py-1 cursor-pointer">
            <span> 回上頁繼續購買 </span>
        </div>
            <div class="flex justify-center items-center bg-[#50468c] text-white rounded-md px-4 py-1 cursor-pointer">
        <span> 確認購買 </span>
        </div>
    </div>
</div>
    </div>
</template>