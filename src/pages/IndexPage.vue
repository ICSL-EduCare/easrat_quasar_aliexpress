<template>
  <div class="bg-white" style="min-height: 100vh; font-family: Arial, sans-serif;">

    <div style="height: 35px;" class="border-bottom"></div>

    <div class="row items-center q-px-xl" style="height: 75px; gap: 25px;">

      <div class="text-h4 text-weight-bold text-cyan-10">
        Ali<span class="text-teal-10">Express</span>
      </div>

      <q-input
        v-model="search"
        outlined
        dense
        color="cyan-10"
        class="col"
        style="max-width: 430px;"
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
        style="font-size: 12px; text-align: center; white-space: nowrap;"
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
            style="width: 300px; border-radius: 15px; padding: 18px;"
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
        style="font-size: 11px; line-height: 16px; padding: 8px 10px;"
      >

        <q-menu>

          <q-card
            style="width: 180px; padding: 15px; border-radius: 12px;"
            class="bg-white"
          >

            <q-btn
              unelevated
              rounded
              no-caps
              label="Sign in"
              color="teal-10"
              style="width: 100%; margin-bottom: 8px;"
            />

            <div
              class="text-cyan-10"
              style="text-align: center; font-size: 11px; margin-bottom: 15px;"
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
      style="height: 48px; margin-bottom: 20px;"
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
      style="height: 30px; display: flex; align-items: center; justify-content: center; font-size: 12px;"
    >

      <q-icon
        name="local_shipping"
        color="cyan-10"
        size="17px"
        style="margin-right: 6px;"
      />

      Free shipping On all Choice items

    </div>

  </div>
</template>

<script setup>
import { ref } from 'vue'

import image1 from 'src/assets/image1.jpg'
import image2 from 'src/assets/image2.jpg'
import image3 from 'src/assets/image3.jpg'

const search = ref('')
const slide = ref('slide1')
</script>

<style scoped>
.border-bottom {
  border-bottom: 1px solid var(--q-cyan-2);
}
</style>
