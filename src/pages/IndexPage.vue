<template>
  <div
    class="bg-white"
    style="min-height: 100vh; font-family: Arial, sans-serif;"
  >

    <div style="height: 35px;" class="border-bottom"></div>

    <div
      class="row items-center q-px-xl"
      style="height: 75px; gap: 35px;"
    >

      <div class="text-h4 text-weight-bold text-cyan-10">
        Ali<span class="text-teal-10">Express</span>
      </div>

      <q-input
        v-model="search"
        rounded
        outlined
        dense
        color="cyan-10"
        class="col"
        style="max-width: 600px;"
        placeholder="1 Cent Items"
      >
        <template v-slot:append>

          <q-icon
            name="image_search"
            color="cyan-10"
            size="20px"
          />

          <q-btn
            round
            unelevated
            dense
            icon="search"
            color="teal-10"
            class="q-ml-sm"
            size="sm"
          />

        </template>
      </q-input>

      <div
        class="text-teal-10"
        style="
          font-size: 12px;
          text-align: center;
          white-space: nowrap;
        "
      >
        <q-icon
          name="smartphone"
          color="cyan-10"
          size="20px"
        />
        <br>
        Download the
        <br>
        AliExpress app
      </div>

      <q-btn
        flat
        dense
        no-caps
        icon="language"
        label="EN / BDT"
        color="teal-10"
        style="font-size: 12px; padding: 8px 10px;"
      >

        <q-menu>
          <q-card
            style="
              width: 300px;
              border-radius: 15px;
              padding: 18px;
            "
            class="bg-white"
          >

            <div class="text-weight-bold text-teal-10 q-mb-sm">
              Ship to
            </div>

            <q-select
              outlined
              dense
              model-value="Bangladesh"
              :options="['Bangladesh']"
              color="cyan-10"
              class="q-mb-md"
            />

            <div class="text-weight-bold text-teal-10 q-mb-sm">
              Language
            </div>

            <q-select
              outlined
              dense
              model-value="English"
              :options="['English']"
              color="cyan-10"
              class="q-mb-md"
            />

            <div class="text-weight-bold text-teal-10 q-mb-sm">
              Currency
            </div>

            <q-select
              outlined
              dense
              model-value="BDT (Bangladeshi Taka)"
              :options="['BDT (Bangladeshi Taka)']"
              color="cyan-10"
              class="q-mb-lg"
            />

            <q-btn
              unelevated
              rounded
              no-caps
              label="Save"
              color="teal-10"
              style="width: 100%;"
            />

          </q-card>
        </q-menu>

      </q-btn>

      <q-btn
        flat
        dense
        no-caps
        icon="person_outline"
        label="Welcome
        Sign in / Register"
        color="teal-10"
        style="
          font-size: 11px;
          line-height: 16px;
          padding: 8px 10px;
        "
      >

        <q-menu>

          <q-card
            style="
              width: 180px;
              padding: 15px;
              border-radius: 12px;
            "
            class="bg-white"
          >

            <q-btn
              unelevated
              rounded
              no-caps
              label="Sign in"
              color="teal-10"
              style="
                width: 100%;
                margin-bottom: 8px;
              "
            />

            <div
              class="text-cyan-10"
              style="
                text-align: center;
                font-size: 11px;
                margin-bottom: 15px;
              "
            >
              Register
            </div>

            <q-list style="font-size: 12px;">

              <q-item clickable>
                <q-item-section avatar>
                  <q-icon name="receipt_long" color="cyan-10" />
                </q-item-section>
                <q-item-section>My Orders</q-item-section>
              </q-item>

              <q-item clickable>
                <q-item-section avatar>
                  <q-icon name="monetization_on" color="cyan-10" />
                </q-item-section>
                <q-item-section>My Coins</q-item-section>
              </q-item>

              <q-item clickable>
                <q-item-section avatar>
                  <q-icon name="chat" color="cyan-10" />
                </q-item-section>
                <q-item-section>Message Center</q-item-section>
              </q-item>

              <q-item clickable>
                <q-item-section avatar>
                  <q-icon name="payments" color="cyan-10" />
                </q-item-section>
                <q-item-section>Payment</q-item-section>
              </q-item>

              <q-item clickable>
                <q-item-section avatar>
                  <q-icon name="favorite_border" color="cyan-10" />
                </q-item-section>
                <q-item-section>Wish List</q-item-section>
              </q-item>

              <q-item clickable>
                <q-item-section avatar>
                  <q-icon name="local_offer" color="cyan-10" />
                </q-item-section>
                <q-item-section>My Coupons</q-item-section>
              </q-item>

            </q-list>

          </q-card>

        </q-menu>

      </q-btn>

      <div
        class="text-teal-10"
        style="font-size: 13px; white-space: nowrap;"
      >

        <q-icon
          name="shopping_cart"
          color="cyan-10"
          size="20px"
        />

        <b>0</b>

        <br>

        <span style="font-size: 11px;">
          Cart
        </span>

      </div>

    </div>


    <div
      class="row items-center justify-between q-px-xl border-bottom"
      style="
        height: 48px;
        margin-bottom: 20px;
      "
    >

      <q-btn
        flat
        rounded
        no-caps
        icon="menu"
        label="All Categories"
        color="teal-10"
        class="bg-cyan-1"
        style="width: 150px;"
      >

        <q-menu>

          <q-list style="width: 200px; padding: 8px 0;">

            <q-item clickable>
              <q-item-section avatar>
                <q-icon name="home" color="cyan-10" />
              </q-item-section>
              <q-item-section>Home & Living</q-item-section>
            </q-item>

            <q-item clickable>
              <q-item-section avatar>
                <q-icon name="directions_car" color="cyan-10" />
              </q-item-section>
              <q-item-section>Automotive</q-item-section>
            </q-item>

            <q-item clickable>
              <q-item-section avatar>
                <q-icon name="kitchen" color="cyan-10" />
              </q-item-section>
              <q-item-section>Appliances</q-item-section>
            </q-item>

            <q-item clickable>
              <q-item-section avatar>
                <q-icon name="checkroom" color="cyan-10" />
              </q-item-section>
              <q-item-section>Women's Clothing</q-item-section>
            </q-item>

            <q-item clickable>
              <q-item-section avatar>
                <q-icon name="person" color="cyan-10" />
              </q-item-section>
              <q-item-section>Men's Clothing</q-item-section>
            </q-item>

            <q-item clickable>
              <q-item-section avatar>
                <q-icon name="toys" color="cyan-10" />
              </q-item-section>
              <q-item-section>Toys & Games</q-item-section>
            </q-item>

            <q-item clickable>
              <q-item-section avatar>
                <q-icon name="chair" color="cyan-10" />
              </q-item-section>
              <q-item-section>Furniture</q-item-section>
            </q-item>

            <q-item clickable>
              <q-item-section avatar>
                <q-icon name="face" color="cyan-10" />
              </q-item-section>
              <q-item-section>Beauty & Health</q-item-section>
            </q-item>

            <q-item clickable>
              <q-item-section avatar>
                <q-icon name="checkroom" color="cyan-10" />
              </q-item-section>
              <q-item-section>Shoes</q-item-section>
            </q-item>

            <q-item clickable>
              <q-item-section avatar>
                <q-icon name="devices" color="cyan-10" />
              </q-item-section>
              <q-item-section>Electronics</q-item-section>
            </q-item>

            <q-item clickable>
              <q-item-section avatar>
                <q-icon name="diamond" color="cyan-10" />
              </q-item-section>
              <q-item-section>Jewelry & Accessories</q-item-section>
            </q-item>

            <q-item clickable>
              <q-item-section avatar>
                <q-icon name="phone_android" color="cyan-10" />
              </q-item-section>
              <q-item-section>Cell Phones & Accessories</q-item-section>
            </q-item>

          </q-list>

        </q-menu>

      </q-btn>

      <q-btn
        flat
        rounded
        no-caps
        label="SuperDeals"
        color="cyan-10"
        style="font-weight: bold; padding: 8px 15px;"
      />

      <q-btn
        flat
        rounded
        no-caps
        label="AliExpress Business"
        color="teal-10"
        style="padding: 8px 15px;"
      />

      <q-btn
        flat
        rounded
        no-caps
        label="Automotive"
        color="teal-10"
        style="padding: 8px 15px;"
      />

      <q-btn
        flat
        rounded
        no-caps
        label="Appliances"
        color="teal-10"
        style="padding: 8px 15px;"
      />

      <q-btn
        flat
        rounded
        no-caps
        label="Women's Clothing"
        color="teal-10"
        style="padding: 8px 15px;"
      />

      <q-btn
        flat
        rounded
        no-caps
        label="Men's Clothing"
        color="teal-10"
        style="padding: 8px 15px;"
      />

      <q-btn
        flat
        rounded
        no-caps
        label="More"
        icon-right="expand_more"
        color="teal-10"
        style="padding: 8px 15px;"
      />

    </div>


    <!-- MAIN BANNER -->
    <div style="padding: 0 20px;">

      <q-carousel
        v-model="slide"
        autoplay
        infinite
        animated
        arrows
        navigation
        transition-prev="slide-right"
        transition-next="slide-left"
        height="300px"
        control-color="cyan-10"
        class="bg-cyan-1"
      >

        <q-carousel-slide
          name="slide1"
          :img-src="image1"
          class="q-pa-none"
        />

        <q-carousel-slide
          name="slide2"
          :img-src="image2"
          class="q-pa-none"
        />

        <q-carousel-slide
          name="slide3"
          :img-src="image3"
          class="q-pa-none"
        />

      </q-carousel>

    </div>


    <div
      class="bg-cyan-1 text-teal-10"
      style="
        height: 30px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 12px;
      "
    >

      <q-icon
        name="local_shipping"
        color="cyan-10"
        size="17px"
        style="margin-right: 6px;"
      />

      Free shipping On all Choice items

    </div>



<div class="q-pa-lg">

  <div class="text-h5 text-weight-bold text-center q-mb-lg">
    Today's deals
  </div>

  <div class="row q-col-gutter-md">

    <div class="col-12 col-md-6">

      <q-card bordered>

        <q-card-section>
          <div class="text-h6 text-weight-bold text-center">
            Bundle deals
          </div>

          <div class="text-center q-mt-sm">
            <q-badge color="orange-2" text-color="orange-10" rounded>
              3 from US $2.99
            </q-badge>
          </div>
        </q-card-section>

        <q-card-section>

          <div class="row q-col-gutter-sm">

            <div class="col-4">
              <q-img :src="productImage" ratio="1" />
              <div class="q-mt-sm text-caption">Star Pendant</div>
              <div class="text-weight-bold text-red">539.25৳</div>
              <div class="text-caption">⭐ 4.9</div>
              <div class="text-caption">5,000+ sold</div>
            </div>

            <div class="col-4">
              <q-img :src="productImage" ratio="1" />
              <div class="q-mt-sm text-caption">Smart Wristband</div>
              <div class="text-weight-bold text-red">766.50৳</div>
              <div class="text-caption">⭐ 4.6</div>
              <div class="text-caption">1,000+ sold</div>
            </div>

            <div class="col-4">
              <q-img :src="productImage" ratio="1" />
              <div class="q-mt-sm text-caption">Kitchen Rack</div>
              <div class="text-weight-bold text-red">637.52৳</div>
              <div class="text-caption">⭐ 4.7</div>
              <div class="text-caption">10,000+ sold</div>
            </div>

          </div>

        </q-card-section>

      </q-card>

    </div>



    <div class="col-12 col-md-6">

      <q-card bordered>

        <q-card-section>

          <div class="text-h6 text-weight-bold text-center">
            SuperDeals
          </div>

          <div class="text-center q-mt-sm">
            <q-badge color="pink-1" text-color="red" rounded>
              Ends in: 23:00:13
            </q-badge>
          </div>

        </q-card-section>

        <q-card-section>

          <div class="row q-col-gutter-sm">

            <div class="col-4">
              <q-img :src="productImage" ratio="1" />
              <div class="q-mt-sm text-caption">Plush Toy</div>
              <div class="text-weight-bold text-red">277.43৳</div>
              <div class="text-caption">⭐ 4.9</div>
              <q-badge color="red">-78%</q-badge>
            </div>

            <div class="col-4">
              <q-img :src="productImage" ratio="1" />
              <div class="q-mt-sm text-caption">Cloud Lamp</div>
              <div class="text-weight-bold text-red">3,578.32৳</div>
              <div class="text-caption">⭐ 4.8</div>
              <q-badge color="red">-10%</q-badge>
            </div>

            <div class="col-4">
              <q-img :src="productImage" ratio="1" />
              <div class="q-mt-sm text-caption">Baby Clothing</div>
              <div class="text-weight-bold text-red">774.65৳</div>
              <div class="text-caption">⭐ 4.7</div>
              <q-badge color="red">-66%</q-badge>
            </div>

          </div>

        </q-card-section>

      </q-card>

    </div>

  </div>

</div>


<div
    class="q-pa-lg"
    :style="{
      backgroundImage: `linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url(${image3})`,
      backgroundSize: 'cover',
      backgroundPosition: 'center',
      minHeight: '500px'
    }"
  >

    <div class="text-h5 text-weight-bold q-mb-lg">
      SuperBuyer
    </div>

    <div class="row q-col-gutter-lg">

      <div class="col-12 col-md-6">
        <q-card>

          <q-card-section>
            <div class="text-h6 text-weight-bold">
              Bulk Saver Hub
            </div>
          </q-card-section>

          <q-card-section>
            <div class="row q-col-gutter-sm">

              <div class="col-4">
                <q-img :src="productImage" ratio="1" />
                <div class="text-weight-bold q-mt-sm">81.02৳</div>
                <div class="text-caption">each, ≥5 pcs</div>
              </div>

              <div class="col-4">
                <q-img :src="productImage" ratio="1" />
                <div class="text-weight-bold q-mt-sm">557.90৳</div>
                <div class="text-caption">each, ≥3 pcs</div>
              </div>

              <div class="col-4">
                <q-img :src="productImage" ratio="1" />
                <div class="text-weight-bold q-mt-sm">92.86৳</div>
                <div class="text-caption">each, ≥10 pcs</div>
              </div>

            </div>
          </q-card-section>

        </q-card>
      </div>

      <div class="col-12 col-md-6">
        <q-card>

          <q-card-section>
            <div class="text-h6 text-weight-bold">
              Buy again
            </div>
          </q-card-section>

          <q-card-section>
            <div class="row q-col-gutter-sm">

              <div class="col-4">
                <q-img :src="productImage" ratio="1" />
                <div class="text-weight-bold q-mt-sm">1,265.23৳</div>
                <div class="text-caption">Popular picks</div>
              </div>

              <div class="col-4">
                <q-img :src="productImage" ratio="1" />
                <div class="text-weight-bold q-mt-sm">362.85৳</div>
                <div class="text-caption">Popular picks</div>
              </div>

              <div class="col-4">
                <q-img :src="productImage" ratio="1" />
                <div class="text-weight-bold q-mt-sm">307.87৳</div>
                <div class="text-caption">Popular picks</div>
              </div>

            </div>
          </q-card-section>

        </q-card>
      </div>

    </div>

  </div>

<div class="q-pa-lg">

  <div class="text-h5 text-weight-bold text-center q-mb-lg">
    Shop by category
  </div>

  <div class="row q-col-gutter-md">

    <div class="col-12 col-md-6">

      <q-card class="bg-cyan-1" style="height: 100%;">

        <q-card-section>

          <div class="row items-center">

            <div class="col-6">

              <div class="text-h4 text-weight-bold">
                Viva
              </div>

              <div class="text-weight-bold">
                Your fashion choice
              </div>

              <q-btn
                unelevated
                no-caps
                color="black"
                label="Shop now"
                class="q-mt-md"
              />

            </div>

          </div>

        </q-card-section>

        <q-card-section>

          <div class="row q-col-gutter-sm">

            <div class="col-4">
              <q-card class="bg-white">
                <q-img :src="productImage" ratio="1" />
                <div class="q-pa-sm">
                  <div class="text-weight-bold">2,469.01৳</div>
                  <div class="text-caption">⭐ 4.5</div>
                  <div class="text-caption">1,000+ sold</div>
                </div>
              </q-card>
            </div>

            <div class="col-4">
              <q-card class="bg-white">
                <q-img :src="productImage" ratio="1" />
                <div class="q-pa-sm">
                  <div class="text-weight-bold">2,469.01৳</div>
                  <div class="text-caption">⭐ 4.5</div>
                  <div class="text-caption">1,000+ sold</div>
                </div>
              </q-card>
            </div>

            <div class="col-4">
              <q-card class="bg-white">
                <q-img :src="productImage" ratio="1" />
                <div class="q-pa-sm">
                  <div class="text-weight-bold">2,469.01৳</div>
                  <div class="text-caption">⭐ 4.5</div>
                  <div class="text-caption">1,000+ sold</div>
                </div>
              </q-card>
            </div>

          </div>

        </q-card-section>
      </q-card>

    </div>

    <div class="col-12 col-md-6">

      <div class="row q-col-gutter-sm">

        <div class="col-6">
          <q-card class="bg-grey-1">
            <q-card-section>
              <div class="row items-center">
                <div class="col-6 text-weight-bold">
                  Women's Clothing
                </div>
                <div class="col-6">
                  <q-img :src="productImage" ratio="1" />
                </div>
              </div>
            </q-card-section>
          </q-card>
        </div>

        <div class="col-6">
          <q-card class="bg-grey-1">
            <q-card-section>
              <div class="row items-center">
                <div class="col-6 text-weight-bold">
                  Men's Clothing
                </div>
                <div class="col-6">
                  <q-img :src="productImage" ratio="1" />
                </div>
              </div>
            </q-card-section>
          </q-card>
        </div>

        <div class="col-6">
          <q-card class="bg-grey-1">
            <q-card-section>
              <div class="row items-center">
                <div class="col-6 text-weight-bold">
                  Toys & Games
                </div>
                <div class="col-6">
                  <q-img :src="productImage" ratio="1" />
                </div>
              </div>
            </q-card-section>
          </q-card>
        </div>

        <div class="col-6">
          <q-card class="bg-grey-1">
            <q-card-section>
              <div class="row items-center">
                <div class="col-6 text-weight-bold">
                  Furniture
                </div>
                <div class="col-6">
                  <q-img :src="productImage" ratio="1" />
                </div>
              </div>
            </q-card-section>
          </q-card>
        </div>

        <div class="col-6">
          <q-card class="bg-grey-1">
            <q-card-section>
              <div class="row items-center">
                <div class="col-6 text-weight-bold">
                  Beauty & Health
                </div>
                <div class="col-6">
                  <q-img :src="productImage" ratio="1" />
                </div>
              </div>
            </q-card-section>
          </q-card>
        </div>

        <div class="col-6">
          <q-card class="bg-grey-1">
            <q-card-section>
              <div class="row items-center">
                <div class="col-6 text-weight-bold">
                  Shoes
                </div>
                <div class="col-6">
                  <q-img :src="productImage" ratio="1" />
                </div>
              </div>
            </q-card-section>
          </q-card>
        </div>

      </div>

    </div>

  </div>

</div>

</div>

<footer>

  <div class="bg-white text-black q-pa-xl">

    <div class="row q-col-gutter-xl">

      <div class="col-12 col-md-6 footer-column">
        <div class="text-h6 text-weight-bold q-mb-md">
          Help
        </div>

        <div class="footer-links">
          <span>Help Center</span>
          <span>Disputes & Reports</span>
          <span>Return & refund policy</span>
          <span>Report IPR infringement</span>
          <span>DSA/OSA Information</span>
          <span>Information and contacts for Brazil</span>
          <span>Integrity Compliance</span>
          <span>Transparency Center</span>
          <span>Submit report (non-registered users)</span>
          <span>Return Policy</span>
        </div>
      </div>


      <!-- AliExpress Multi-Language Sites -->
      <div class="col-12 col-md-6 footer-column">
        <div class="text-h6 text-weight-bold q-mb-md">
          AliExpress Multi-Language Sites
        </div>

        <div class="footer-links">
          <span>Russian</span>
          <span>Portuguese</span>
          <span>Spanish</span>
          <span>French</span>
          <span>German</span>
          <span>Italian</span>
          <span>Dutch</span>
          <span>Turkish</span>
          <span>Japanese</span>
          <span>Korean</span>
          <span>Thai</span>
          <span>Arabic</span>
          <span>Hebrew</span>
          <span>Polish</span>
        </div>
      </div>


      <!-- Browse by Category -->
      <div class="col-12 col-md-6 footer-column">
        <div class="text-h6 text-weight-bold q-mb-md">
          Browse by Category
        </div>

        <div class="footer-links">
          <span>All Popular</span>
          <span>Product</span>
          <span>Promotion</span>
          <span>Low Price</span>
          <span>Great Value</span>
          <span>Reviews</span>
          <span>Wiki</span>
          <span>Blog</span>
          <span>Video</span>
        </div>
      </div>


      <!-- Alibaba Group -->
      <div class="col-12 col-md-6 footer-column">
        <div class="text-h6 text-weight-bold q-mb-md">
          Alibaba Group
        </div>

        <div class="footer-links">
          <span>Alibaba Group Website</span>
          <span>AliExpress</span>
          <span>Alimama</span>
          <span>Fliggy</span>
          <span>Alibaba Cloud</span>
          <span>Alibaba International</span>
          <span>AliTelecom</span>
          <span>DingTalk</span>
          <span>Juhuasuan</span>
          <span>Taobao Marketplace</span>
          <span>Tmall</span>
          <span>Taobao Global</span>
          <span>AliOS</span>
          <span>1688</span>
        </div>
      </div>

    </div>

  </div>


  <div
    class="bg-grey-10 text-grey-4 q-pa-lg"
    style="font-size: 11px; line-height: 1.8;"
  >

    <div class="text-center">

      <div>
        Intellectual Property Protection -
        Privacy Policy -
        Sitemap -
        Terms of Use -
        Information for EU consumers -
        <strong>Legal Information / Imprint</strong> -
        Transaction Services Agreement for non-EU/UK Consumers -
        Terms and Conditions for EU/EEA/UK Consumers -
      </div>

      <div class="q-mt-sm">
        User Information Legal Enquiry Guide&nbsp;&nbsp;
        ©️ 2010-2025 AliExpress.com. All rights reserved.&nbsp;
        🌐 增值电信业务经营许可证 浙B2-20120091-8&nbsp;
        🔴 浙公网安备33010802014622号&nbsp;
        浙ICP备2024067534号-11
      </div>

    </div>

  </div>

</footer>
</template>


<script setup>
import { ref } from 'vue'

import image1 from 'src/assets/image1.jpg'
import image2 from 'src/assets/image2.jpg'
import image3 from 'src/assets/image3.jpg'
import productImage from 'src/assets/product-image.png'

const search = ref('')
const slide = ref('slide1')
</script>

<style scoped>
.border-bottom {
  border-bottom: 1px solid var(--q-cyan-2);
}
</style>
