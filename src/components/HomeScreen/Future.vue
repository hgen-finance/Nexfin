<template>
  <div class="container pt-8-L pt-8-M pt-15-S pt-20-XS px-20-XS mb-40-S">
    <div
      class="w-100 fd-r-S fd-c-XS ai-c jc-l-S jc-c-XS rad-fix-8 px-14-S px-20-XS py-10-S py-20-XS"
    >
    <div class="w-100 d-n-S fd-r jc-c">
      <div class="w-100 mb-20-XS fd-r jc-c">
        <AmButton
            color="gradient-5002"
            opacityEffect
            scaleEffect
            disableShadow
            :full="mobile"
            link="https://dev.hgen.finance"
            v-if="!publicKey"
          >
            Launch App
          </AmButton>
      </div>
    </div>
      <div class="w-50-S w-100-XS">
        <div class = "w-100 fd-r">
          <div
          class="w-100 tt-u fs-18-S fs-40-XS fw-600 ta-l-S ta-c-XS pt-0-M pt-2-S pt-2-XS"
          >
          Connecting <br/> Value and ESG
          </div>
          <div class ="fd-r ai-c">
            <img
            src="@/assets/svg/earth.svg"
            class="h-fix-40-S h-fix-20-S h-fix-100-XS"
            />
          </div>
        </div>
       
        <div
          class="w-100 fs-6-S fs-20-XS fw-400 f-lh-18-S f-lh-45-XS pt-4-S pt-15-XS ta-l-S ta-c-XS pb-15-XS"
        >
          HGEN is a blockchain-based DeFi platform that supports not only financial returns but also social and global environmental imporvement through quick and easy impact investment in hydrogen energy industry.
        </div>
        <div
          class="w-100 fd-r-S fd-c-XS mt-0-L mt-0-M mt-5-S pt-6-M pt-0-S pt-6-XS d-f-S d-n-XS"
        >
          <AmButton
            class=""
            color="gradient-5002"
            bColor="gradient-5002"
            colorText="white-200"
            opacityEffect
            disableShadow
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
<script>
</script>
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
