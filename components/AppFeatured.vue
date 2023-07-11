<template lang="">
  <div class="mt-10">
    <Chips>Featured Collections</Chips>
    <Chips>Apparel</Chips>
    <Chips>Shoes</Chips>
    <div class="mx-2 flex overflow-x-scroll mt-2">
      <Itemcard
        v-for="item in data"
        :key="data.id"
        :propsitem="item"
        :propstype="'featured'"
      />
    </div>
  </div>
</template>
<script>
export default {
  setup() {
    const { data, error } = useFetch(
      'https://fakestoreapi.com/products?limit=10/category/men%27s%20clothing'
    );
    return { data, error };
  },
};
</script>
<style lang=""></style>
