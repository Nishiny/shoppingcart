<script >
export default {

  data() {
    return {
    
    }
  },

  methods:{

  },

}
</script>

<template>
  <div class="w-full p-3 px-5">
      <div>
        <h1 class="mb-3 text-3xl font-bold">完成購買 </h1>
      </div>
      <div class="mb-6 px-5">
        <div class="grid-table">
          <div class="grid-thead">
            <div class="grid-cols-4 grid border-y border-main-deep text-main-deep font-bold py-1 gap-x-3">
              <div class="gird-th text-center">商品圖片</div>
              <div class="gird-th">商品名稱</div>
              <div class="gird-th text-center">價錢</div>
              <div class="gird-th text-center">數量</div>
            </div>
          </div>
          <div class="grid-tbody">
            <div class="grid-tr grid-cols-4 grid py-1 border-b border-main-deep min-h-[80px] gap-x-3">
              <div class="flex justify-center">
                <img src="../assets/image/300x300_0.png" alt="商品圖示" class="w-[100px] h-full ">
              </div>
              <div class="flex items-center">Bytecard</div>
              <div class="gird-td flex justify-center items-center"> $954</div>
              <div class="gird-td flex justify-center items-center ">
                <div class="card-btns-list flex-col">2</div>
              </div>
            </div>
          </div>
        </div>
      </div>
  </div>
  <div class="mb-6 px-5">
    <div class="grid-table">
      <div class="grid-thead">
        <div class="grid-cols-6 grid border-y border-main-deep text-main-deep font-bold py-1 gap-x-3">
          <div class="gird-th">姓名</div>
          <div class="gird-th">電話</div>
          <div class="gird-th">地址</div>
          <div class="gird-th">付款方式</div>
          <div class="gird-th">電子信箱</div>
          <div class="gird-th">運送方式</div>
        </div>
      </div>
        <div class="grid-tbody">
            <div class="grid-tr grid-cols-6 grid py-1 border-b border-main-deep min-h-[80px] gap-x-3">
              <div class="flex items-center">3124</div>
              <div class="flex items-center">8687</div>
              <div class="flex items-center">5624</div>
              <div class="flex items-center">貨到付款</div>
              <div class="flex items-center">5323@ghgee</div>
              <div class="flex items-center">超商取貨</div>
            </div>
        </div>
      </div>
      <a href="#/shopping" class="flex justify-center items-center bg-[#50468c] text-white rounded-md px-4 py-1 cursor-pointer">
        <span> 回首頁 </span>
      </a>
    </div>
</template>