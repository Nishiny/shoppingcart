<script >
export default {
  data() {
   
  },

  methods:{
  },
}
</script>

<template>
<div class="w-full p-3 px-5">
    <div>
        <h1 class="mb-3 text-3xl font-bold">購買確認及填寫資訊</h1>
    </div>
    <div class="grid-thead pb-3">
            <div class="grid-cols-4 grid border-y border-main-deep text-main-deep font-bold py-1 gap-x-3">
                <div class="gird-th text-center">商品圖片</div>
                <div class="gird-th text-center">商品</div>
                <div class="gird-th">$$$</div>
            </div>
        </div>
        <form>
            <div class="mb-6 px-5">
                <label for="name" class="block mb-2 text-lg font-bold">姓名</label>
                <input type="text" id="name" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:border-indigo-500" required="">
            </div>
            <div class="mb-6 px-5">
                <label for="phone" class="block mb-2 text-lg font-bold">電話</label>
                <input type="text" id="phone" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:border-indigo-500" required="">
            </div>
            <div class="mb-6 px-5">
                <label for="address" class="block mb-2 text-lg font-bold">地址</label>
                <input type="text" id="address" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:border-indigo-500" required="">
            </div>
            <div class="mb-6 px-5">
                <label for="email" class="block mb-2 text-lg font-bold">電子信箱</label>
                <input type="email" id="email" class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:border-indigo-500" required="">
            </div>
            <div class="mb-6 px-5">
                <label for="paymentMethod" class="block mb-2 text-lg font-bold">付款方式</label>
                <div class="flex gap-5">
                    <div class="flex items-center">
                        <input type="radio" class="mr-2">
                        <label for="paymentMethod1">信用卡</label>
                    </div>
                    <div class="flex items-center">
                    <input type="radio" class="mr-2">
                    <label for="paymentMethod2">貨到付款</label>
                    </div>
                </div>
            </div>
            <div class="mb-6 px-5">
                <label for="shippingMethod" class="block mb-2 text-lg font-bold">運送方式</label>
                <div class="flex gap-5">
                    <div class="flex items-center">
                        <input type="radio" class="mr-2">
                        <label for="shippingMethod1">宅配</label>
                    </div>
                    <div class="flex items-center">
                        <input type="radio" class="mr-2" >
                        <label for="shippingMethod2">超商取貨</label>
                    </div>
                </div>
            </div>
        </form>
        <div class="flex justify-end flex-wrap mb-5">
            <h2 class="text-2xl font-bold w-full text-end">商品數量:0 </h2>
            <h2 class="text-2xl font-bold w-full text-end">商品金額:$0 </h2>
        </div>
        <div class="w-full flex justify-between">
            <div class="flex justify-center items-center bg-[#8c5046] text-white rounded-md px-4 py-1 cursor-pointer">
                <span> 回上頁繼續加購 </span>
            </div>
            <button type="submit" class="flex justify-center items-center bg-[#50468c] text-white rounded-md px-4 py-1 cursor-pointer">
                <span>確認送出</span>
            </button>
        </div>
</div>

</template>