<template>
  <div class="container pt-20-M pt-20-S mb-0-S mb-10-XS jc-c ai-c-XS fd-c">
    <div class="w-100 ml-20-S pl-30-L pl-10-M pl-30-S mt-30-L mt-18-M mt-9-S pt-17-S ai-c-XS">
      <div class="fw-500 fs-9-M fs-10-S ta-c-XS">P2P DEFI PLATFORM</div>
      <div class="fw-800 cus-f fs-30-M fs-30-S ta-c-XS">HGEN</div>
    </div>
    <div class="pt-20-XS mt-0-S pt-0-S pl-0-M pl-20-S pt-12-S pl-12-L">
      <div class="fw-600 fs-14-M fs-10-S fs-20-XS pb-5-S pb-10-XS">
        Realisation of customer value <br />
        through connection with decentralisaton and transparency
      </div>
      <div class="w-60-S w-100-XS mb-5-S mb-10-XS fs-6-M fs-8-S fs-20-XS">
        HGEN which is based on stability + profitability, focuses on providing a decentralised and transparent platform.
      </div>
    </div>
    <div
      class="w-100 pt-30-XS fd-r fd-c-XS jc-c px-0-M pt-5-S pb-0-S px-20-XS mt-20-S"
    >
      <div
        class="w-100-M w-100-S w-100-XS p-8-M p-10-S p-20-XS"
        v-for="(item, i) in hydrogenItems"
        :key="i"
      >
        <div class="w-100 fs-12-M fs-10-S fs-25-XS fw-600" v-html="item.name" />
        <p v-html="item.text" class="pt-3-S pt-10-XS fs-5-M fs-8-S fs-18-XS" />
        <div class="w-100 pt-4-S pt-10-XS">
          <div
            class="w-100 fd-r ai-t py-2-M py-3-S py-5-XS fs-5-M fs-8-S fs-18-XS"
            v-for="(item2, i2) in item.items"
            :key="i2"
          >
            <img
              :src="require('@/assets/svg/' + item2.img)"
              class="h-fix-s-9-M h-fix-s-7-S h-fix-s-20-XS mr-2-S mr-5-XS"
            />
            <span v-html="item2.name" />
          </div>
        </div>
      </div>
    </div>

    <div class="w-100 fd-c jc-c mt-30-S jc-c">
      <div class="mt-30-M mt-10-S"></div>
      <div class="mt-30-M mt-10-S"></div>
      <div class="mt-30-M mt-10-S"></div>
      <div class="mt-30-M mt-10-S"></div>
      <div class="mt-10-M mt-5-S"></div>
      <img
        src="@/assets/svg/SOL_logo.svg"
        class="h-fix-100-S h-fix-20-S h-fix-35-XS d-n-XS"
      />
      <div class="fs-10-S ta-c f-white-200">
        <span class="fw-600">HGEN</span> operates on
        <span class="fw-600">SOLANA</span>
      </div>
    </div>
    <div class="w-100 fd-c jc-c ai-c">
      <div class="mt-30-M mt-10-S"></div>
      <div class="mt-30-M mt-10-S"></div>
      <div class="mt-10-M mt-5-S"></div>
      <div class="ta-c fs-10-M fw-400 f-white-200 mb-10-M">
        Connecting people and their Investment Value
      </div>
      <div class="line h-fix-30-M py-10-M"></div>
      <img
        src="@/assets/svg/HGEN_logo_1.svg"
        class="h-fix-100-S h-fix-20-S h-fix-150-XS"
      />
      <div class="line h-fix-30-M py-10-M my-5-M"></div>
      <div class="mt-5-M mt-5-S"></div>
      <div class="w-100 f-gray-400 ta-c fs-6-S fs-25-XS py-20-XS fw-500">
        Total Deposited Value
      </div>
      <div
        class="w-100 f-white-200 tt-u fs-20-S fs-30-XS fw-900 ta-c pt-4-S pt-15-X glow mb-20-XS"
      >
        $ {{ getTotal }}
      </div>
    </div>
    <div class="w-100 fd-c ai-c">
      <div
        class="w-50-S w-100-XS fd-c-S fd-c-XS ai-c jc-l-S jc-c-XS gradient-1000 rad-fix-8 px-14-S px-20-XS py-10-S py-20-XS my-10-S"
      >
        <div
          class="w-100 tt-u fs-11-S fs-25-XS f-white-200 fw-600 ta-c pt-0-M pt-2-S pt-2-XS"
        >
          Q3 of 2022 on mainnet
        </div>
        <div
          class="w-100 fs-6-S fs-20-XS f-gray-500 fw-400 f-lh-18-S f-lh-45-XS pt-4-S pt-15-XS ta-c pb-15-XS"
        >
          We are ready on solana Devnet.
          <br />
          Be one of the first to experience it by participating in Devnet and
          receive rewards.

          <!-- We have a strong integrated solution to bring our world to DeFi online
            platform, greatly reduces risks and environmental pollution, and
            results in more reliable power through the utilization of existing
            engineering art. -->
        </div>
      </div>
    </div>
    <div class="w-100 fd-c ai-c mt-10-M mt-40-XS">
      <div
        class="w-100 f-white-200 tt-u fs-17-S fs-30-XS fw-800 ta-c glow"
        data-aos="zoom-in"
      >
        <i>Growth With Purpose</i>
      </div>
      <div class="w-100 fd-r jc-c pt-5-M pt-20-XS px-0-S px-20-XS">
        <AmButton color="gradient-5002" bColor="gradient-5002" opacityEffect link="https://docs.hgen.finance/beginners-guide">
          <div class="w-100 tt-n fs-6-S fs-18-XS fw-600">Beginner’s Guide</div>
        </AmButton>
      </div>
      <div class="w-75 f-white-200 py-5-M fs-6-M fs-20-XS mt-10-XS">
        We have strong integrated solution to bring our web2.0 services to DeFi platform. Bridging gaps among web2 and web3.
      </div>
      <div
        class="w-100 f-white-200 pt-30-XS jc-c px-0-M pt-5-S pb-0-S px-10-XS mt-10-S my-col-3-S my-col-1-XS"
        data-aos-ease="ease"
      >
        <div
          class="w-100-M  w-100-S w-100-XS p-5-M p-10-S p-20-XS gradient-1000 rad-fix-10 shadow-cyan-200"
          data-aos-ease="ease"
          data-aos-delay="200"
          v-for="(item, i) in ProjectItems"
          :key="i"
        >
          <div
            class="w-100 f-cyan-600 fs-12-M fs-10-S fs-25-XS fw-600"
            v-html="item.name"
          />
          <p
            v-html="item.text"
            class="pt-3-S pt-10-XS fs-5-M fs-8-S fs-18-XS"
          />
          <div class="w-100 pt-4-S pt-10-XS">
            <div
              class="w-100 fd-r ai-t py-2-M py-3-S py-5-XS fs-5-M fs-8-S fs-18-XS"
              v-for="(item2, i2) in item.items"
              :key="i2"
            >
              <img
                :src="require('@/assets/svg/' + item2.img)"
                class="h-fix-s-9-M h-fix-s-7-S h-fix-s-20-XS mr-2-S mr-5-XS"
              />
              <span v-html="item2.name" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          img: "defiFuture1.svg",
          name: "Borrowing",
          text: "Get an interes-free loan",
        },
        {
          img: "defiFuture2.svg",
          name: "Safe Pool",
          text: "We have triple earnings.",
        },
        {
          img: "defiFuture3.svg",
          name: "Farming",
          text: "Fund to earn transaction fees profit.",
        },
      ],
      hydrogenItems: [
        {
          name: "Impact Investment",
          text: 'With the intention of generating financial returns beyond investing in companies, organisation and funds "Investing in consideration of social and environment nurition"',
          img: "roadMap1.png",
          items: [],
        },
        // {
        //   name: "Hydrogen Industry",
        //   text: "The market of opportunity to grow over next 80 years. As of the end of 2021, the hydrogen infrastructure will be worth USD 142 billion. By 2025, it is expected to grow at a rapid CAGR of 9.2% to USD 2010 billion. It is a market of growing opportunity",
        //   img: "roadMap2.png",
        //   items: [],
        // },
        {
          name: "Defi Platform",
          text: "HGEN is a blockchain based DEfi platform that supports not only financial returns but also social and environmental improvement through quick and easy impact investment.",
          img: "roadMap3.png",
          items: [],
        },
      ],
      ProjectItems: [
        {
          name: "Borrow & Staking",
          text: "The borrowing & Staking will be a critical component to the $HGEN DeFi Project Financing Platform",
          img: "roadMap1.png",
          items: [
            {
              img: "checkOn.svg",
              name: "Get an interests-free loan with Borrow",
            },
            { img: "checkOn.svg", name: "Get triple earnings with Staking" },
            {
              img: "checkOn.svg",
              name: "Leverage investments possible through",
            },
            { img: "checkOn.svg", name: "minting $GENS stablecoin" },
          ],
        },
        {
          name: "Farms",
          text: "The farming will give you additional benefit.",
          img: "roadMap2.png",
          items: [
            {
              img: "checkOn.svg",
              name: "Fund to earn transaction fees profit",
            },
            // {
            //   img: "checkOn.svg",
            //   name: "Funding for Hydrogen Industries",
            // },
            {
              img: "checkOn.svg",
              name: "Support cross platform",
            },
          ],
        },
        // {
        //   name: "Hydrogen Project Financing",
        //   text: "The $HGEN DeFi Platform will focus on the growth of the hydrogen market by offering project financing capabilities to entities seeking to be part of, or grow the hydrogen ecosystem.",
        //   img: "roadMap3.png",
        //   items: [{ img: "checkOn.svg", name: "PF based staking fund" }],
        // },
        // {
        //   name: "Big Data (Hydrogen Focused Data)",
        //   text: "Hydrogen cars registered on the platform will be connected to the $HGEN network of data. Including hydrogen charging stations, hydrogen consumption usage, and the ability to pay using $HGEN/$GENS Tokens. e.g.",
        //   img: "roadMap3.png",
        //   items: [
        //     {
        //       img: "checkOn.svg",
        //       name: " Hydrogen vehicle data aggregator",
        //     },
        //     {
        //       img: "checkOn.svg",
        //       name: "Vehicle-specific private / public keys provided",
        //     },
        //     {
        //       img: "checkOn.svg",
        //       name: "Find the location of Hydrogen Recharge",
        //     },
        //     { img: "checkOn.svg", name: "View hydrogen fuel prices" },
        //     {
        //       img: "checkOn.svg",
        //       name: "Rechargeable fuel (line) can be settled",
        //     },
        //   ],
        // },
        // {
        //   name: "Smart (Micro) Grid",
        //   text: "Green hydrogen based energy can be connected to local ESS (Energy Storage Systems). Thereby allowing individuals to buy green energy directly from the producer, and providing energy providers with a method of selling power.",
        //   img: "roadMap3.png",
        //   items: [
        //     {
        //       img: "checkOn.svg",
        //       name: "Real-time energy tracking and measurement capabilities",
        //     },
        //     {
        //       img: "checkOn.svg",
        //       name: "Power trading system between ESS to prevent energy shortage and overheating",
        //     },
        //     {
        //       img: "checkOn.svg",
        //       name: "Operating Energy Tracking and Trading system",
        //     },
        //     {
        //       img: "checkOn.svg",
        //       name: "Activating Aggregator for EVs and Charge stations",
        //     },
        //     { img: "checkOn.svg", name: "P2P Energy Trading" },
        //     { img: "checkOn.svg", name: "More to Announced" },
        //   ],
        // },
      ],
    };
  },
  
};
</script>

<style lang="scss" scoped>


.cus-f {
  font-family: "koHo";
}

.line {
  background-color: white;
  width: 1px;
}
</style>
