<template>
  <q-page
    class="bg-grey-4 flex flex-center"
    style="
      width:100vw;
      height:100vh;
      padding:28px;
      box-sizing:border-box;
      overflow:hidden;
    "
  >

    <div
      style="
        width:min(100%,1250px);
        height:min(100%,690px);
        display:grid;
        grid-template-columns:repeat(3,1fr);
        grid-template-rows:repeat(3,1fr);
        gap:38px 58px;
      "
    >

      <q-card
        class="bg-white"
        style="
          position:relative;
          overflow:hidden;
          border-radius:0;
          box-shadow:0 5px 9px rgba(0,0,0,.15);
        "
      >
        <div
          class="absolute-full q-ma-sm"
          style="border:1px solid #ccc;"
        >
          <div
            class="bg-gradient"
            style="
              position:absolute;
              left:18%;
              top:23%;
              width:6px;
              height:50%;
            "
          ></div>

          <div
            style="
              position:absolute;
              left:28%;
              top:30%;
            "
          >
            <div
              class="text-black text-weight-bold"
              style="
                font-size:clamp(20px,2vw,32px);
                line-height:.9;
              "
            >
              DESIGN<br>
              PORTFOLIO
            </div>

            <div
              class="text-grey-7"
              style="
                margin-top:10px;
                font-size:7px;
              "
            >
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
            </div>
          </div>

          <div
            class="bg-grey-10"
            style="
              position:absolute;
              right:0;
              bottom:8%;
              width:45px;
              height:12px;
            "
          ></div>

          <div
            class="bg-grey-10"
            style="
              position:absolute;
              right:50px;
              bottom:8%;
              width:5px;
              height:12px;
            "
          ></div>

          <div
            class="bg-grey-10"
            style="
              position:absolute;
              right:58px;
              bottom:8%;
              width:5px;
              height:12px;
            "
          ></div>
        </div>
      </q-card>


      <q-card
        class="bg-white"
        style="
          position:relative;
          overflow:hidden;
          border-radius:0;
          box-shadow:0 5px 9px rgba(0,0,0,.15);
        "
      >
        <div
          style="
            position:absolute;
            left:0;
            top:0;
            width:55%;
            height:100%;
          "
          class="bg-blue-grey-2"
        ></div>

        <q-img
          :src="image"
          style="
            position:absolute;
            right:0;
            top:0;
            width:46%;
            height:100%;
          "
          fit="cover"
        />

        <div
          class="absolute text-white"
          style="
            left:15%;
            bottom:12%;
            width:42%;
            padding:14px;
            box-sizing:border-box;
            border:1px solid white;
          "
        >
          <div
            class="text-weight-bold"
            style="
              font-size:clamp(12px,1.2vw,20px);
              line-height:.9;
            "
          >
            ABOUT<br>
            DESIGN
          </div>

          <div
            style="
              margin-top:8px;
              font-size:6px;
              line-height:1.5;
            "
          >
            Creative ideas and thoughtful visual experiences.
          </div>
        </div>

        <div
          class="absolute text-white text-weight-bold"
          style="
            top:6%;
            left:7%;
            font-size:9px;
          "
        >
          ━━━
        </div>
      </q-card>


      <q-card
        class="bg-white"
        style="
          position:relative;
          overflow:hidden;
          border-radius:0;
          box-shadow:0 5px 9px rgba(0,0,0,.15);
        "
      >
        <q-img
          :src="image"
          class="absolute-full"
          fit="cover"
        />

        <div
          class="bg-purple-2"
          style="
            position:absolute;
            right:8%;
            top:7%;
            width:27%;
            height:23%;
            opacity:.85;
          "
        ></div>

        <div
          class="bg-white"
          style="
            position:absolute;
            left:7%;
            bottom:14%;
            padding:7px 12px;
          "
        >
          <div
            class="text-black text-weight-bold"
            style="
              font-size:clamp(12px,1.2vw,20px);
            "
          >
            STYLE DESIGN
          </div>

          <div
            class="text-grey-7"
            style="
              margin-top:5px;
              font-size:6px;
            "
          >
            Lorem ipsum dolor sit amet, consectetur adipiscing elit.
          </div>
        </div>

        <div
          class="bg-grey-10"
          style="
            position:absolute;
            right:0;
            bottom:8%;
            width:45px;
            height:12px;
          "
        ></div>
      </q-card>


      <q-card
        class="bg-white"
        style="
          position:relative;
          overflow:hidden;
          border-radius:0;
          box-shadow:0 5px 9px rgba(0,0,0,.15);
        "
      >
        <q-img
          :src="image"
          class="absolute-full"
          fit="cover"
        />

        <div
          class="bg-purple-2"
          style="
            position:absolute;
            left:38%;
            top:18%;
            width:32%;
            height:63%;
            opacity:.9;
          "
        ></div>

        <div
          style="
            position:absolute;
            left:43%;
            top:29%;
          "
        >
          <div
            class="text-black text-weight-bold"
            style="
              font-size:clamp(13px,1.4vw,22px);
              line-height:.9;
            "
          >
            DESIGN<br>
            CREATIVE
          </div>

          <div
            class="text-grey-8"
            style="
              width:100px;
              margin-top:7px;
              font-size:6px;
              line-height:1.5;
            "
          >
            Creative solutions built with simplicity and elegance.
          </div>
        </div>

        <div
          class="bg-grey-10"
          style="
            position:absolute;
            right:0;
            bottom:8%;
            width:45px;
            height:12px;
          "
        ></div>
      </q-card>


      <q-card
        class="bg-white"
        style="
          position:relative;
          overflow:hidden;
          border-radius:0;
          box-shadow:0 5px 9px rgba(0,0,0,.15);
        "
      >
        <div
          class="bg-blue-grey-2"
          style="
            position:absolute;
            left:0;
            top:0;
            width:34%;
            height:20%;
          "
        ></div>

        <q-img
          :src="image"
          style="
            position:absolute;
            left:0;
            bottom:0;
            width:40%;
            height:78%;
          "
            fit="cover"
        />

        <div
          style="
            position:absolute;
            left:29%;
            top:29%;
            width:63%;
          "
        >
          <div
            class="text-black text-weight-bold"
            style="
              font-size:clamp(22px,2.3vw,38px);
              line-height:.9;
            "
          >
            GRAPHIC<br>
            STUDIO
          </div>

          <div
            class="text-grey-8"
            style="
              margin-top:8px;
              width:70%;
              font-size:6px;
              line-height:1.5;
            "
          >
            Design creates the connection between imagination and communication.
          </div>
        </div>

        <q-img
          :src="image"
          style="
            position:absolute;
            right:5%;
            bottom:7%;
            width:23%;
            height:30%;
          "
          fit="cover"
        />

        <div
          class="bg-purple-2"
          style="
            position:absolute;
            right:0;
            bottom:0;
            width:34%;
            height:20%;
            opacity:.7;
          "
        ></div>
      </q-card>


      <q-card
        class="bg-white"
        style="
          position:relative;
          overflow:hidden;
          border-radius:0;
          box-shadow:0 5px 9px rgba(0,0,0,.15);
        "
      >
        <div
          style="
            position:absolute;
            left:7%;
            top:17%;
            z-index:3;
          "
        >
          <div
            class="text-black text-weight-bold"
            style="
              font-size:clamp(13px,1.4vw,22px);
            "
          >
            GRAPHIC DESIGN
          </div>

          <div
            class="text-grey-8"
            style="
              width:65%;
              margin-top:7px;
              font-size:6px;
              line-height:1.5;
            "
          >
            Great design combines creativity, balance and purpose.
          </div>
        </div>

        <q-img
          :src="image"
          style="
            position:absolute;
            left:0;
            bottom:0;
            width:58%;
            height:58%;
          "
          fit="cover"
        />

        <q-img
          :src="image"
          style="
            position:absolute;
            right:3%;
            top:5%;
            width:37%;
            height:76%;
            transform:rotate(-3deg);
          "
          fit="cover"
        />

        <div
          class="bg-blue-grey-2"
          style="
            position:absolute;
            right:0;
            bottom:14%;
            width:8%;
            height:28%;
          "
        ></div>

        <div
          class="bg-grey-10"
          style="
            position:absolute;
            right:0;
            bottom:8%;
            width:45px;
            height:12px;
          "
        ></div>
      </q-card>


      <q-card
        class="bg-white"
        style="
          position:relative;
          overflow:hidden;
          border-radius:0;
          box-shadow:0 5px 9px rgba(0,0,0,.15);
        "
      >
        <div
          style="
            position:absolute;
            inset:12px;
            border:1px solid #bbb;
          "
        ></div>

        <q-img
          :src="image"
          style="
            position:absolute;
            left:8%;
            top:8%;
            width:84%;
            height:84%;
          "
          fit="cover"
        />

        <div
          class="text-grey-8"
          style="
            position:absolute;
            right:6%;
            top:8%;
            writing-mode:vertical-rl;
            font-size:5px;
            letter-spacing:1px;
          "
        >
          CREATIVE STUDIO
        </div>
      </q-card>


      <q-card
        class="bg-white"
        style="
          position:relative;
          overflow:hidden;
          border-radius:0;
          box-shadow:0 5px 9px rgba(0,0,0,.15);
        "
      >
        <div
          style="
            position:absolute;
            left:0;
            top:0;
            bottom:0;
            width:27%;
            display:grid;
            grid-template-rows:repeat(3,1fr);
            gap:2px;
          "
        >
          <q-img :src="image" fit="cover" />
          <q-img :src="image" fit="cover" />
          <q-img :src="image" fit="cover" />
        </div>

        <div
          style="
            position:absolute;
            left:31%;
            right:8%;
            top:12%;
          "
        >
          <div
            style="
              display:grid;
              grid-template-columns:25px 1fr;
              gap:8px;
              margin-bottom:12px;
            "
          >
            <div
              class="text-black text-weight-bold"
              style="font-size:17px;"
            >
              1.
            </div>

            <div
              class="text-grey-8"
              style="
                font-size:6px;
                line-height:1.5;
              "
            >
              Research your subject and understand the purpose of the project.
            </div>
          </div>

          <div
            style="
              display:grid;
              grid-template-columns:25px 1fr;
              gap:8px;
              margin-bottom:12px;
            "
          >
            <div
              class="text-black text-weight-bold"
              style="font-size:17px;"
            >
              2.
            </div>

            <div
              class="text-grey-8"
              style="
                font-size:6px;
                line-height:1.5;
              "
            >
              Create a clear visual concept using balanced colors and spacing.
            </div>
          </div>

          <div
            style="
              display:grid;
              grid-template-columns:25px 1fr;
              gap:8px;
            "
          >
            <div
              class="text-black text-weight-bold"
              style="font-size:17px;"
            >
              3.
            </div>

            <div
              class="text-grey-8"
              style="
                font-size:6px;
                line-height:1.5;
              "
            >
              Complete the final design and present it professionally.
            </div>
          </div>
        </div>

        <div
          class="bg-grey-10"
          style="
            position:absolute;
            right:0;
            top:25%;
            width:8px;
            height:50%;
          "
        ></div>
      </q-card>


      <q-card
        class="bg-white"
        style="
          position:relative;
          overflow:hidden;
          border-radius:0;
          box-shadow:0 5px 9px rgba(0,0,0,.15);
        "
      >
        <div
          class="bg-purple-2"
          style="
            position:absolute;
            left:0;
            top:0;
            width:53%;
            height:67%;
          "
        ></div>

        <div
          style="
            position:absolute;
            right:12%;
            top:16%;
            width:43%;
            height:58%;
            border:1px solid #aaa;
          "
        ></div>

        <div
          style="
            position:absolute;
            left:28%;
            top:30%;
            z-index:2;
          "
        >
          <div
            class="text-black text-weight-bold"
            style="
              font-size:clamp(20px,2vw,32px);
              line-height:.9;
            "
          >
            THANK<br>
            YOU
          </div>

          <div
            class="text-grey-7"
            style="
              margin-top:8px;
              font-size:6px;
            "
          >
            Lorem ipsum dolor sit amet.
          </div>
        </div>

        <div
          class="bg-grey-10"
          style="
            position:absolute;
            right:0;
            bottom:8%;
            width:45px;
            height:12px;
          "
        ></div>

        <div
          class="bg-grey-10"
          style="
            position:absolute;
            right:50px;
            bottom:8%;
            width:5px;
            height:12px;
          "
        ></div>

        <div
          class="bg-grey-10"
          style="
            position:absolute;
            right:58px;
            bottom:8%;
            width:5px;
            height:12px;
          "
        ></div>
      </q-card>

    </div>
  </q-page>
</template>

<script setup>
import image from 'src/assets/image.png'
</script>
