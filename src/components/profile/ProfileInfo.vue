<template>
  <v-card
    flat
    class="product-card"
  >
    <img
      class="product-image"
      :src="product.image"
      :alt="product.product_name"
    />

    <v-card-text>
      <div class="product-name">
        {{ product.product_name }}
      </div>

      <div class="product-description">
        {{ product.product_description }}
      </div>

      <div class="product-price">
        ฿{{ product.price }}
      </div>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  name: 'ProductCard',

  props: {
    product: {
      type: Object,
      required: true
    }
  }
}
</script>

<style scoped>
.product-card {
  border-radius: 18px;
  overflow: hidden;
}

.product-image {
  width: 100%;
  height: 220px;
  object-fit: cover;
}

.product-name {
  font-size: 18px;
  font-weight: 600;
}

.product-description {
  margin-top: 6px;
  color: #777;
  font-size: 14px;
}

.product-price {
  margin-top: 12px;
  font-size: 18px;
  font-weight: 600;
}
</style>