<template>
        <div class="col-md-8">
      <h2 class="mb-3">商品列表</h2>
      <div class="row">
        <div v-for="product in products" :key="product.id" class="col-md-4 mb-4">
          <div class="card h-100">
            <img :src="product.images" class="card-img-top">
            <div class="card-body">
              <h5 class="card-title">耳罩式藍牙耳機</h5>
              <p class="card-text">舒適配戴，支援降噪技術</p>
              <p class="fw-bold text-primary">$ 2490</p>
              <button class="btn btn-success w-100"> 加入購物車 </button>
            </div>
          </div>
        </div>
      </div>
    </div>
    {{ products }}
</template>


<script setup>
const props= defineProps({
    products:{
        type:Array,
        required: true,
    },
})

</script>