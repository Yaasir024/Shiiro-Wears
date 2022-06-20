<template>
  <main>
    <header>
      <h2>CART</h2>
    </header>
    <section class="cart">
      <table>
        <tr>
          <th>Product</th>
          <th>Quantity</th>
          <th>Total</th>
        </tr>
        <tr>
          <td>
            <div class="product-details">
              <img src="../assets/image/cargo.webp" alt="" class="cart-img" />
              <div>
                <p class="product-name">T-shirt white</p>
                <p class="variation">M</p>
                <span class="product-price"> $100 </span>
                <br />
                <button class="remove-btn">Remove</button>
              </div>
            </div>
          </td>
          <td><input type="number" value="1" /></td>
          <td>$100</td>
        </tr>
        <tr>
          <td>
            <div class="product-details">
              <img src="../assets/image/sneaker.webp" alt="" class="cart-img" />
              <div>
                <p class="product-name">Teh Sneakers</p>
                <span class="product-price"> $100 </span>
                <br />
                <button class="remove-btn">Remove</button>
              </div>
            </div>
          </td>
          <td><input type="number" value="1" /></td>
          <td>$100</td>
        </tr>
      </table>
      <div>
        <div class="total-container">
          <table>
            <tr>
              <td>Subtotal</td>
              <td>$200</td>
            </tr>
            <tr>
              <td>Tax</td>
              <td>$20</td>
            </tr>
            <tr>
              <td>Total</td>
              <td>$220</td>
            </tr>
          </table>
          <br />
        </div>
          <div class="btn-container">
            <button class="black-btn">CHECK OUT</button>
          </div>
      </div>
    </section>
  </main>
</template>

<script>
export default {};
</script>

<style scoped>
main {
  padding: 0 20px;
}
header {
  text-align: center;
  margin: 50px 0;
}
header h2 {
  font-weight: 700;
  font-size: 24px;
}
.cart {
  max-width: 950px;
  margin: 0 auto;
}
table {
  width: 100%;
  border-collapse: collapse;
}
.product-details {
  display: flex;
  flex-wrap: wrap;
}
.product-name {
  margin-top: 5px;
}
th {
  text-align: left;
  padding: 5px;
  color: #fff;
  background: var(--color-dark);
  font-weight: normal;
}
td {
  padding: 10px 5px;
}
td input {
  width: 40px;
  height: 30px;
  padding: 5px;
}
.cart-img {
  max-width: 100px;
  max-height: 120px;
  margin-right: 10px;
}
.remove-btn {
  background: none;
  border: none;
  padding: 8px 14px;
  transition: all 0.3s ease-in-out;
  cursor: pointer;
  border: 1px solid var(--color-dark);
  /* color: #fff; */
}
.remove-btn:hover {
  background: var(--color-dark);
  color: #fff;
}
.total-container {
  display: flex;
  justify-content: flex-end;
}
.total-container table {
  border-top: 3px solid var(--color-dark);
  width: 100%;
  max-width: 380px;
}
td:last-child {
  text-align: right;
}
th:last-child {
  text-align: right;
}
.btn-container
{
  display: flex;
  justify-content: flex-end;
  margin-top: 20px;
}
.black-btn {
  background: var(--color-dark);
  border: none;
  padding: 15px 14px;
  width: 100%;
  max-width: 380px;
  transition: all 0.3s ease-in-out;
  cursor: pointer;
  border: 1px solid var(--color-dark);
  color: #fff;
}
.black-btn:hover {
  background: none;
  color: var(--text-color);
}
</style>
