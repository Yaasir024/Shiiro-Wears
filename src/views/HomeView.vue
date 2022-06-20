<script setup></script>

<template>
  <main>
    <section class="product-section">
      <div class="title-wrapper">
        <h1 class="title">New Releases</h1>
      </div>
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
              <img
                class="product-img"
                src="../assets/image/cargo.webp"
                alt=""
              />
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
              <img
                class="product-img"
                src="../assets/image/cargo.webp"
                alt=""
              />
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
              <img
                class="product-img"
                src="../assets/image/cargo.webp"
                alt=""
              />
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
              <img
                class="product-img"
                src="../assets/image/cargo.webp"
                alt=""
              />
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
              <img
                class="product-img"
                src="../assets/image/cargo.webp"
                alt=""
              />
            </div>
            <div class="product-meta">
              <h2 class="product-title">Cargo Pants</h2>
              <p class="product-price">$150</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="product-section">
      <div class="category-container">
        <div class="category-item">
          <img src="../assets/image/cargo.webp" alt="" class="category-img" />
          <div class="category-title">
            <span>Pants</span>
          </div>
        </div>
        <div class="category-item">
          <img src="../assets/image/sneaker.webp" alt="" class="category-img" />
          <div class="category-title">
            <span>Sneaker</span>
          </div>
        </div>
        <div class="category-item">
          <img src="../assets/image/cargo.webp" alt="" class="category-img" />
          <div class="category-title">
            <span>Pants</span>
          </div>
        </div>
        <div class="category-item">
          <img src="../assets/image/sneaker.webp" alt="" class="category-img" />
          <div class="category-title">
            <span>Sneaker</span>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<style scoped>
.product-section {
  padding: 0 15px;
}
.title-wrapper {
  margin: 30px 0;
}
.title-wrapper .title {
  font-size: 20px;
  font-weight: 600;
}

/* Items Container */
.products-container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
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
  left: 0;
}

/* Category */
.category-container {
  display: flex;
  flex-wrap: wrap;
  margin: 80px 0;
}
.category-item {
  position: relative;
  /* flex: 0 0 25%; */
  width: 25%;
  padding: 5px 15px;
}
.category-img {
  width: 100%;
}
.category-title {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  left: 50%;
  transform: translateX(-50%);
  text-align: center;
}
.category-title span {
  padding: 8px 15px;
  color: #fff;
  display: inline-block;
  background-color: #00000054;
}
@media screen and (max-width: 750px) {
  .category-item {
    flex: 0 0 50%;
    width: 50%;
  }
}
</style>
