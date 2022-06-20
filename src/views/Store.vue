<template>
  <main class="main">
    <header>
      <h2>SHIRTS</h2>
    </header>
    <div class="products-container">
      <div class="product">
        <div class="card-wrapper">
          <div class="image-wrapper">
            <img
              class="product-img"
              src="../assets/image/sneaker.webp"
              alt=""
            />
          </div>
          <div class="product-meta">
            <h2 class="product-title">Sneaker</h2>
            <p class="product-price">$100</p>
          </div>
          <span class="product-tag">Out of Stock</span>
        </div>
      </div>
      <div class="product">
        <div class="card-wrapper">
          <div class="image-wrapper">
            <img class="product-img" src="../assets/image/cargo.webp" alt="" />
          </div>
          <div class="product-meta">
            <h2 class="product-title">Cargo Pants</h2>
            <p class="product-price">$150</p>
          </div>
        </div>
      </div>
      <div class="product">
        <div class="card-wrapper">
          <div class="image-wrapper">
            <img
              class="product-img"
              src="../assets/image/sneaker.webp"
              alt=""
            />
          </div>
          <div class="product-meta">
            <h2 class="product-title">Sneaker</h2>
            <p class="product-price">$100</p>
          </div>
          <span class="product-tag">Out of Stock</span>
        </div>
      </div>
      <div class="product">
        <div class="card-wrapper">
          <div class="image-wrapper">
            <img class="product-img" src="../assets/image/cargo.webp" alt="" />
          </div>
          <div class="product-meta">
            <h2 class="product-title">Cargo Pants</h2>
            <p class="product-price">$150</p>
          </div>
        </div>
      </div>
      <div class="product">
        <div class="card-wrapper">
          <div class="image-wrapper">
            <img
              class="product-img"
              src="../assets/image/sneaker.webp"
              alt=""
            />
          </div>
          <div class="product-meta">
            <h2 class="product-title">Sneaker</h2>
            <p class="product-price">$100</p>
          </div>
          <span class="product-tag">Out of Stock</span>
        </div>
      </div>
      <div class="product">
        <div class="card-wrapper">
          <div class="image-wrapper">
            <img class="product-img" src="../assets/image/cargo.webp" alt="" />
          </div>
          <div class="product-meta">
            <h2 class="product-title">Cargo Pants</h2>
            <p class="product-price">$150</p>
          </div>
        </div>
      </div>
      <div class="product">
        <div class="card-wrapper">
          <div class="image-wrapper">
            <img
              class="product-img"
              src="../assets/image/sneaker.webp"
              alt=""
            />
          </div>
          <div class="product-meta">
            <h2 class="product-title">Sneaker</h2>
            <p class="product-price">$100</p>
          </div>
          <span class="product-tag">Out of Stock</span>
        </div>
      </div>
      <div class="product">
        <div class="card-wrapper">
          <div class="image-wrapper">
            <img class="product-img" src="../assets/image/cargo.webp" alt="" />
          </div>
          <div class="product-meta">
            <h2 class="product-title">Cargo Pants</h2>
            <p class="product-price">$150</p>
          </div>
        </div>
      </div>
      <div class="product">
        <div class="card-wrapper">
          <div class="image-wrapper">
            <img
              class="product-img"
              src="../assets/image/sneaker.webp"
              alt=""
            />
          </div>
          <div class="product-meta">
            <h2 class="product-title">Sneaker</h2>
            <p class="product-price">$100</p>
          </div>
          <span class="product-tag">Out of Stock</span>
        </div>
      </div>
      <div class="product">
        <div class="card-wrapper">
          <div class="image-wrapper">
            <img class="product-img" src="../assets/image/cargo.webp" alt="" />
          </div>
          <div class="product-meta">
            <h2 class="product-title">Cargo Pants</h2>
            <p class="product-price">$150</p>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {};
</script>

<style scoped>
main{
    padding: 0 20px;
}
header {
    margin: 40px 0;
}
header h2 {
    font-weight: 700;
    font-size: 24px;
}

/* Items Container */
.products-container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  grid-gap: calc(2em + 2vh) calc(1.5em + 1vmin);
  grid-auto-flow: row dense;
}
.card-wrapper {
  position: relative;
}
.product-img {
  max-width: 100%;
}
.product-meta {
  text-align: center;
}
.product-title {
  font-size: 20px;
  font-weight: 600;
}
.product-price {
  margin-top: 5px;
  font-size: 12px;
}
.product-tag {
  background: var(--text-color);
  color: #fff;
  padding: 5px;
  font-size: 14px;
  position: absolute;
  top: 0;
  right: 0;
}
</style>
