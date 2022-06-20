<template>
  <main>
    <header>
        <h2>CART</h2>
    </header>
    <section class="cart">
        <div class="cart-row-header">
            <div class="header-item-container">
                <div class="header-item">
                    Quantity
                </div>
                <div class="header-item">
                    Total
                </div>
            </div>
        </div>
    </section>
  </main>
</template>

<script>
export default {

}
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
.cart-row-header {
    margin-bottom: 1px solid var(--border-color2);
    padding-bottom: 15px;
}
.header-item-container {
    float: left;
    left: 60%;
    min-height: 1px;
}
.header-item {
    float: left;
    width: 50%;
        min-height: 1px;
        text-align: center;
}
</style>