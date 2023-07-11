<template lang="">
  <div class="rounded-lg w-[300px] min-w-[300px] border mx-1 shadow-lg">
    <img
      :src="propsitem.image"
      class="mx-auto mt-1 rounded h-48 w-full object-contain"
    />
    <div class="m-2">
      <h2>{{ propsitem.title }}</h2>
      <p>{{ propsitem.price }}</p>
      <p>{{ propsitem.rating.rate }}</p>
    </div>
    <div class="flex justify-between mx-2" v-if="propstype !== 'featured'">
      <button class="bg-slate-600 rounded p-2 text-white w-full">
        Add to Cart
      </button>
      <button class="bg-gray-400 rounded p-2 text-white w-full">Buy now</button>
    </div>
  </div>
</template>
<script>
export default {
  props: ['propsitem', 'propstype'],

  data() {
    return {
      item: [],
      type: '',
    };
  },
  setup({ propsitem, propstype }) {
    // this.item = propsitem;
    // this.type = propstype;
    // console.log(propstype);
  },
};
</script>
<style lang=""></style>
