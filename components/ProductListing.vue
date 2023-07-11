<template lang="">
  <div class="mx-2 mt-10">
    <h1 class="underline">All Products</h1>
    <div class="mx-2 flex overflow-auto mt-2">
      <Itemcard
        v-for="item in data"
        :key="data.id"
        :propsitem="item"
        :propstype="'all'"
      />
    </div>
    <div class="flex justify-center mt-5">
      <button class="bg-slate-600 text-white p-3 text-center rounded-md w-48">
        Browse All
      </button>
    </div>
  </div>
</template>
<script>
export default {
  setup() {
    const { data, error } = useFetch(
      'https://fakestoreapi.com/products/category/jewelery'
    );
    return { data, error };
  },
};
</script>
<style lang=""></style>
