<template>
  <div class="container pt-8-L pt-8-M pt-15-S pt-20-XS px-20-XS">
    <div
      class="w-100 fd-r-S fd-c-XS ai-c jc-l-S jc-c-XS gradient-1000 rad-fix-8 px-14-S px-20-XS py-10-S py-20-XS"
    >
      <div class="w-50-S w-100-XS">
        <div class="w-100-S">
          <!-- <Particles
            id="tsparticles"
            :options="{
              fpsLimit: 60,
              particles: {
                color: {
                  value: '#8E24AA'
                },
                move: {
                  enable: true
                },
                links: {
                  enable: true,
                  color: '#ba63ff'
                }
              }
            }"
          /> -->
        </div>
        <div
          class="w-100 tt-u fs-11-S fs-25-XS f-white-200 fw-600 ta-l-S ta-c-XS pt-0-M pt-2-S pt-2-XS"
        >
          Q3 of 2022 on mainnet
        </div>
        <div
          class="w-100 fs-6-S fs-20-XS f-gray-500 fw-400 f-lh-18-S f-lh-45-XS pt-4-S pt-15-XS ta-l-S ta-c-XS pb-15-XS"
        >
          We are ready on solana Devnet.
          <br />
          Be one of the first to experience it by participating in Devnet and
          receive rewards.
          <br/>
          <ul>
            <li><a
            href="https://nexfin-4wk8byqlc-pree-side.vercel.app"
            class="fw-400 fs-6-L fs-6-M fs-6-S fs-6-XS f-mcolor-300 wb-br-all mt-3"
          >
            New home page desgin
          </a></li>
          <li><a
            href="https://nexfin-web-ui.vercel.app"
            class="fw-400 fs-6-L fs-6-M fs-6-S fs-6-XS f-mcolor-300 wb-br-all mt-3"
          >
            New App desgin
          </a></li>
          </ul>
         

          <!-- We have a strong integrated solution to bring our world to DeFi online
          platform, greatly reduces risks and environmental pollution, and
          results in more reliable power through the utilization of existing
          engineering art. -->
        </div>
        <div
          class="w-100 fd-r-S fd-c-XS mt-0-L mt-0-M mt-5-S pt-6-M pt-0-S pt-6-XS d-f-S d-n-XS"
        >
          <AmButton
            class=""
            color="mcolor-100"
            bColor="mcolor-100"
            colorText="mcolor-400"
            opacityEffect
            link="https://hgen-finance.medium.com"
          >
            HGEN story on <span class="fw-800">Medium</span>
          </AmButton>
        </div>
      </div>
      <!-- <img src="@/static/future.png" class="w-40-S w-80-XS p-a-S p-r-XS l-55-S l-0-XS t-a-S t-fix-5-XS" /> -->
    </div>
  </div>
</template>
<style lang="scss" scoped>
#tsparticles {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  z-index: 0; // 1 layer above the background
}

ul {
  list-style-type: none;
}

ul li {
  padding-left: 30px;
}

ul li:before {
  font-weight: 600;
  font-size: 20px;
  content: "▹";
  position: absolute;
  left: 0px;
  color: purple;
}
</style>
