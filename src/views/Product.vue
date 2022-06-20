<template>
  <main>
    <section class="product-description">
      <div class="image-section">
        <div class="thumbnail">
          <div class="thumbnail-content">
            <div class="thumbnail-item">
                <img class="product-img" src="../assets/image/cargo.webp" alt="" />
            </div>
            <div class="thumbnail-item">
                <img class="product-img" src="../assets/image/cargo.webp" alt="" />
            </div>
            <div class="thumbnail-item">
                <img class="product-img" src="../assets/image/cargo.webp" alt="" />
            </div>
            <div class="thumbnail-item">
                <img class="product-img" src="../assets/image/cargo.webp" alt="" />
            </div>
            <div class="thumbnail-item">
                <img class="product-img" src="../assets/image/cargo.webp" alt="" />
            </div>
            <div class="thumbnail-item">
                <img class="product-img" src="../assets/image/cargo.webp" alt="" />
            </div>
          </div>
        </div>
        <div class="image-wrapper">
          <img class="product-img" src="../assets/image/cargo.webp" alt="" />
        </div>
      </div>
      <div class="details-section">
        <div class="product-meta">
          <div class="meta-head">
            <h2 class="product-category">Accessories /</h2>
            <h1 class="product-name">Black Cargo Trunks</h1>
            <span class="product-price"> $129 </span>
          </div>
          <hr />
          <div class="product-variation">
            <h1>Size:</h1>

            <button>Add to cart</button>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
export default {};
</script>

<style scoped>
img {
  width: 100%;
}
main {
  padding: 0 20px;
}
.product-description {
  margin-top: 20px;
  display: flex;
}
.image-section {
  flex: 0 0 50%;
  width: 50%;
  display: flex;
}
.details-section {
  flex: 0 0 50%;
  width: 50%;
  padding-left: 20px;
}

.thumbnail {
  flex: 0 0 80px;
  max-width: 80px;
  margin-right: 10px;
}
.thumbnail-content {
    max-height: 400px;
    overflow: scroll;
}
.thumbnail-content::-webkit-scrollbar {
    display: none;
}
.thumbnail-content .thumbnail-item {
    margin-bottom: 6px;
}
.image-wrapper {
  max-height: 420px;
  background: #000;
}
.image-wrapper img {
  width: 100%;
}

/* Details Section  */
.product-category {
  font-size: 12px;
  font-weight: 400;
}
.product-name {
  font-size: 20px;
  font-weight: 600;
  margin-bottom: 4px;
}
.product-price {
  font-size: 12px;
  font-weight: 400;
}
</style>
