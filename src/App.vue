<template>
  <div id="app">
    <header
      class="d-flex flex-column flex-md-row align-items-center p-3 px-md-4 mb-4 bg-body border-bottom shadow-sm"
    >
      <p class="h3 my-1 me-md-auto fw-normal">Phone Shop</p>
    </header>
    <main class="container">
      <div class="pricing-header px-3 py-3 pt-md-5 pb-md-4 mx-auto text-center">
        <div class="row row-cols-1 row-cols-md-3 mb-3 text-center">

          <!-- รายการ1 -->
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ pro1.name }}</h4>
              </div>
              <div class="card-body">
                <img
                  src="https://store.ais.co.th/media/catalog/product/t/h/th-iphone_12_pro_max_gold_296x416.png"
                  width="200"
                  height="“200”"
                />
                <ul class="list-unstyled text-small">
                  39,990 บาท
                </ul>
                <div id="example-1">
                  <button
                    type="button"
                    class="w-50 btn btn-lg btn-outline-primary"
                    v-on:click="pro1.amount += 1"
                  >
                    เลือกสินค้า
                  </button>
                  <p>จำนวน {{ pro1.amount }} กล่อง</p>
                </div>
              </div>
            </div>
          </div>

          <!-- รายการ2 -->
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ pro2.name }}</h4>
              </div>
              <div class="card-body">
                <img
                  src="https://www.mobile57.com/product_images/webp/Vivo-Y50_1.webp"
                  width="220"
                  height="“300”"
                />
                <ul class="list-unstyled text-small">
                  8,125 บาท
                </ul>
                <div id="example-2">
                  <button
                    type="button"
                    class="w-50 btn btn-lg btn-outline-primary"
                    v-on:click="pro2.amount += 1"
                  >
                    เลือกสินค้า
                  </button>
                  <p>จำนวน {{ pro2.amount }} กล่อง</p>
                </div>
              </div>
            </div>
          </div>

          <!-- รายการ3 -->
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ pro3.name }}</h4>
              </div>
              <div class="card-body">
                <img
                  src="https://www.mobile57.com/product_images/webp/OPPO-A93-5G-official_1.webp"
                  width="220"
                  height="“300”"
                />
                <ul class="list-unstyled text-small">
                  10,400 บาท
                </ul>
                <div id="example-3">
                  <button
                    type="button"
                    class="w-50 btn btn-lg btn-outline-primary"
                    v-on:click="pro3.amount += 1"
                  >
                    เลือกสินค้า
                  </button>
                  <p>จำนวน {{ pro3.amount }} กล่อง</p>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- รายการ4 -->
        <div class="row row-cols-1 row-cols-md-3 mb-3 text-center">
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ pro4.name }}</h4>
              </div>
              <div class="card-body">
                <img
                  src="https://www.mobile57.com/product_images/webp/galaxy-a02s-product.webp"
                />
                <ul class="list-unstyled text-small">
                  5,525 บาท
                </ul>
                <div id="example-4">
                  <button
                    type="button"
                    class="w-50 btn btn-lg btn-outline-primary"
                    v-on:click="pro4.amount += 1"
                  >
                    เลือกสินค้า
                  </button>
                  <p>จำนวน {{ pro4.amount }} กล่อง</p>
                </div>
              </div>
            </div>
          </div>

          <!-- รายการ5 -->
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ pro5.name }}</h4>
              </div>
              <div class="card-body">
                <img
                  src="https://www.mobile57.com/product_images/webp/poco-m3_1.webp"
                />
                <ul class="list-unstyled text-small">
                  4,990 บาท
                </ul>
                <div id="example-5">
                  <button
                    type="button"
                    class="w-50 btn btn-lg btn-outline-primary"
                    v-on:click="pro5.amount += 1"
                  >
                    เลือกสินค้า
                  </button>
                  <p>จำนวน {{ pro5.amount }} กล่อง</p>
                </div>
              </div>
            </div>
          </div>

          <!-- รายการที่6 -->
          <div class="col">
            <div class="card mb-4 shadow-sm">
              <div class="card-header">
                <h4 class="my-0 fw-normal">{{ pro6.name }}</h4>
              </div>
              <div class="card-body">
                <img
                  src="https://www.mobile57.com/product_images/webp/OnePlus-8_2.webp"
                />
                <ul class="list-unstyled text-small">
                  16,500 บาท
                </ul>
                <div id="example-6">
                  <button
                    type="button"
                    class="w-50 btn btn-lg btn-outline-primary"
                    v-on:click="pro6.amount += 1"
                  >
                    เลือกสินค้า
                  </button>
                  <p>จำนวน {{ pro6.amount }} กล่อง</p>
                </div>
              </div>
            </div>
          </div>
        </div>


        <p class="h4 my-0 me-md-auto fw-normal">ตะกร้าสินค้า</p>
        <header
          class="d-flex flex-column flex-md-row align-items-mide p-3 px-md-4 mb-3 bg-body border-bottom shadow-sm"
        >

          <div v-if="pro1.amount >= 1">
            <img
              src="https://store.ais.co.th/media/catalog/product/t/h/th-iphone_12_pro_max_gold_296x416.png"
              width="60"
              height="“60”"
            />
            <p1> x{{ pro1.amount }} </p1>
          </div>

          <div v-if="pro2.amount >= 1">
            <img
              src="https://www.mobile57.com/product_images/webp/Vivo-Y50_1.webp"
              width="60"
              height="“60”"
            />
            <p1> x{{ pro2.amount }}</p1>
          </div>

          <div v-if="pro3.amount >= 1">
            <img
              src="https://www.mobile57.com/product_images/webp/OPPO-A93-5G-official_1.webp"
              width="60"
              height="“60”"
            />
            <p1> x{{ pro3.amount }}</p1>
          </div>

          <div v-if="pro4.amount >= 1">
            <img
              src="https://www.mobile57.com/product_images/webp/galaxy-a02s-product.webp"
              width="60"
              height="“60”"
            />
            <p1> x{{ pro4.amount }}</p1>
          </div>

          <div v-if="pro5.amount >= 1">
            <img
              src="https://www.mobile57.com/product_images/webp/poco-m3_1.webp"
              width="60"
              height="“60”"
            />
            <p1> x{{ pro5.amount }}</p1>
          </div>

          <div v-if="pro6.amount >= 1">
            <img
              src="https://www.mobile57.com/product_images/webp/OnePlus-8_2.webp"
              width="60"
              height="“60”"
            />
            <p1> x{{ pro6.amount }}</p1>
          </div>

        </header>
        
        <h4>
          ราคาที่ต้องชำระ
          {{
            sum +
            pro1.amount * pro1.price +
            pro2.amount * pro2.price +
            pro3.amount * pro3.price +
            pro4.amount * pro4.price +
            pro5.amount * pro5.price +
            pro6.amount * pro6.price
          }}
          บาท
        </h4>
        <button
          type="button"
          class="w-50 btn btn-lg btn-outline-primary"
          v-on:click="say('ชำระเงินเสร็จสิ้น')"
        >
          ชำระเงิน
        </button>
        <input
          type="button"
          value="Reset"
          onClick="javascript:location.reload();"
        />
      </div>
    </main>
  </div>
</template> 

<script>
export default {
  name: "App",
  data() {
    return {
      pro1: {
        name: "Iphone 12 Pro Max (128GB)",
        price: 39990,
        amount: 0,
      },
      pro2: {
        name: "Vivo Y50",
        price: 8125,
        amount: 0,
      },
      pro3: {
        name: "Oppo A93 5G",
        price: 10400,
        amount: 0,
      },
      pro4: {
        name: "Samsung Galaxy A02s",
        price: 5525,
        amount: 0,
      },
      pro5: {
        name: "Xiaomi Poco M3",
        price: 4990,
        amount: 0,
      },
      pro6: {
        name: "Oneplus 8",
        price: 16500,
        amount: 0,
      },
      sum: 0,
      count: 0,
      say: function (text) {
        alert(text);
      },
    };
  },
};
</script>