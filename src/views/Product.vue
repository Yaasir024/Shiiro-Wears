<template>
  <main>
    <section class="product-description">
      <div class="image-section">
        <div class="thumbnail">
          <div class="thumbnail-content">
            <div class="thumbnail-item">
              <img
                class="product-img"
                src="../assets/image/cargo.webp"
                alt=""
              />
            </div>
            <div class="thumbnail-item">
              <img
                class="product-img"
                src="../assets/image/cargo.webp"
                alt=""
              />
            </div>
            <div class="thumbnail-item">
              <img
                class="product-img"
                src="../assets/image/cargo.webp"
                alt=""
              />
            </div>
            <div class="thumbnail-item">
              <img
                class="product-img"
                src="../assets/image/cargo.webp"
                alt=""
              />
            </div>
            <div class="thumbnail-item">
              <img
                class="product-img"
                src="../assets/image/cargo.webp"
                alt=""
              />
            </div>
            <div class="thumbnail-item">
              <img
                class="product-img"
                src="../assets/image/cargo.webp"
                alt=""
              />
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
            <span>Size</span>
            <div class="variations">
              <div class="variation-item">S</div>
              <div class="variation-item">M</div>
              <div class="variation-item">L</div>
              <div class="variation-item">XL</div>
            </div>

            <button class="black-btn">Add to cart</button>
          </div>
        </div>
        <div class="description-section">
          <div class="tabs">
            <button
              class="tab-btn active"
              :class="description ? 'active' : 'inactive'"
              @click="showDescription"
            >
              Description
            </button>
            <button class="tab-btn" :class="shipping ? 'active' : 'inactive'" @click="showShipping">
              Shipping
            </button>
            <button class="tab-btn" :class="chart ? 'active' : 'inactive'" @click="showChart">
              Size Chart
            </button>
          </div>
          <div class="description" :class="description ? 'show' : 'hide'">
            <div
              class="description-content"
              :class="showFull ? 'showfull' : 'showless'"
            >
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Placeat
                iste recusandae laborum, magnam ipsum cumque similique sint
                necessitatibus voluptatum hic sit ratione expedita unde
                praesentium quam atque ab nisi, deserunt ad impedit, repellat
                consectetur! Nesciunt iusto modi ut odit. Dignissimos, illum,
                quia porro consectetur eius nam aut doloribus iste est, atque
                voluptatem quisquam reprehenderit dicta in? Iusto ratione
                molestiae ea inventore dolore libero repudiandae veniam iste ab
                minima! Voluptatibus, ullam? Perferendis modi optio eveniet
                totam mollitia quam, obcaecati quod officiis quidem doloremque
                at ea deserunt, iste dolor atque sit. Deserunt ab iusto dolorem
                magni alias, sint impedit pariatur laudantium tenetur
                consequuntur. Non, ut sed veritatis alias repellendus sit, neque
                laudantium porro rem suscipit quae nam. Adipisci quisquam at et
                nesciunt, odit molestiae unde beatae dolor nisi repellendus cum
                consequatur, recusandae cumque, tempora delectus. Dolorum porro
                sapiente facilis ipsa nostrum sed ea laudantium! Harum rerum
                delectus magni dolores est provident quidem!
              </p>
            </div>
            <button class="view-btn" @click="showFullContent">
              <p v-if="showFull == false">View More +</p>
              <p v-if="showFull == true">View Less -</p>
            </button>
          </div>
          <div class="shipping" :class="shipping ? 'show' : 'hide'">
            <div class="shipping-content">
              <p>
                Please note that due to COVID-19, our shipping times may have
                delay depending on your country. Your items will be delivered
                within: 2 to 3 weeks for the USA and Canada. 1 to 2 weeks for
                European countries. 2 to 4 weeks for the rest of the world. Feel
                free to reach our team if you have any question: info@shadxw.com
              </p>
            </div>
          </div>
          <div class="size-chart" :class="chart ? 'show' : 'hide'">
            <div class="size-chart-content">
              <p>
                Our team advise you to take one size up on this item to ensure
                your correct size. Some clothing may vary from these
                measurements, if the item has its own measurements table, please
                refer to it
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="reccomendation">
      
    </section>
  </main>
</template>

<script setup>
import { ref, reactive, onMounted } from "vue";
const showFull = ref(false);
const description = ref(true);
const shipping = ref(false);
const chart = ref(false);

const showFullContent = () => {
  showFull.value = !showFull.value;
};
const showDescription = () => {
  description.value = true;
  shipping.value = false;
  chart.value = false;
};
const showShipping = () => {
  description.value = false;
  shipping.value = true;
  chart.value = false;
};
const showChart = () => {
  description.value = false;
  shipping.value = false;
  chart.value = true;
};
</script>

<style scoped>
img {
  width: 100%;
}
main {
  padding: 0 20px;
  max-width: 990px;
  margin: 0 auto;
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
  height: 420px;
  background: #000;
}
.image-wrapper img {
  width: 100%;
  height: 100%;
}

/* Details Section  */
.product-meta .meta-head {
  padding-bottom: 10px;
}
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
  font-size: 14px;
  font-weight: 400;
}
.product-variation {
  margin-top: 20px;
}
.product-variation span {
  margin-bottom: 10px;
  margin-left: 4px;
  font-size: 17px;
  font-weight: 400;
}
.product-variation .variations {
  margin-top: 5px;
}
.product-variation .variation-item {
  padding: 7px 15px;
  font-weight: 400;
  border: 2px solid var(--text-color);
  display: inline-block;
  margin: 0 5px;
}
.black-btn {
  background: var(--color-dark);
  border: none;
  padding: 15px 14px;
  margin-top: 20px;
  width: 100%;
  /* max-width: 380px; */
  transition: all 0.3s ease-in-out;
  cursor: pointer;
  border: 1px solid var(--color-dark);
  color: #fff;
}
.black-btn:hover {
  background: none;
  color: var(--text-color);
}

/* Description Section */
.tabs {
  margin-top: 5px;
}
.tab-btn {
  background-color: #fff;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 10px 16px;
  transition: 0.3s;
  color: gray;
  font-size: 14px;
  width: 33.3333%;
  border-bottom: 2px solid transparent;
}
.active {
  border-bottom: 2px solid var(--color-dark);
  color: var(--color-dark);
}
.inactive {
  border-bottom: 2px solid transparent;
  color: gray;
}
.description,
.shipping,
.size-chart {
  padding: 20px;
  text-align: left;
}
.description-content {
  overflow: hidden;
  transition: max-height 0.3s ease-in-out;
}
.showfull {
  max-height: 1500px;
}
.showless {
  max-height: 150px;
}

.description .view-btn {
  margin: 0 auto;
  width: 100%;
  display: block;
  background: none;
  border: none;
  cursor: pointer;
  transition: background 0.5s, font-weight 0.25s, text-shadow 0.3s,
    transform 0.3s, margin 0.3s;
  background-image: linear-gradient(
    120deg,
    rgba(47, 47, 47, 0.1),
    rgba(47, 47, 47, 0.1)
  );
  background-repeat: no-repeat;
  background-size: 100px 45%;
  background-position: 50% 200%;
  transform: translateY(0px);
  padding: 14px 0;
}
.description .view-btn p {
  font-size: 14px;
}
.shipping {
  display: none;
}
.size-chart {
  display: none;
}
.show {
  display: block;
}
.hide {
  display: none;
}
/* Media Query */
@media screen and (max-width: 750px) {
  .product-description {
    flex-direction: column;
  }
  .image-section,
  .details-section {
    width: 100%;
  }
  .image-section {
    flex-direction: column;
  }
  .thumbnail {
    display: none;
  }
  .details-section {
    text-align: center;
    margin-top: 20px;
  }
}
</style>
