<script >
import CountAdd from '@/components/CountAdd.vue';
export default {
  components:{
    CountAdd,
  },

  data() {
    return {
      add:0,
    };
  },
  methods:{
    changAdd(e){
      this.add = e;
    }
  },
}
</script>

<template>
  {{ add }}
  <br>
  <CountAdd :button-text="'點擊'" :button-number="20" @submit="changAdd"></CountAdd>
</template>
