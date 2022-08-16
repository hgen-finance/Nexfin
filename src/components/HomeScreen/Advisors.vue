<template>
  <div class="container pt-20-S pt-40-XS pb-10-S pb-0-XS">
    <div
      class="w-100 fd-r jc-c ai-c fs-17-S fs-30-XS f-white-200 fw-800 tt-u glow"
      data-aos="zoom-in"
    >
      <i>Team</i>
    </div>
    <div class="w-100 pt-15-S pt-20-XS fd-c jc-c fw-w px-5-S px-0-XS">
      <div
        class="w-95-S w-100-XS fd-r ai-t p-2-S p-20-XS mb-5-S mb-10-XS"
        v-for="(item, i) in items"
        :key="i"
      >
        <div v-if="item.logo">
          <img
            :src="require('@/assets/svg/' + item.logo)"
            class="z-12 w-fix-40-M w-fix-45-S w-fix-100-XS p-a b-90-S b-90-XS my-logo-align"
          />
        </div>
        <div
          class="w-20-S w-60-XS h-fix-95-M h-fix-s-150-XS brs-s br-mcolor-100 shadow-purple-100 ovh rad-fix-6"
        >
          <div v-if="item.img">
            <img
              :src="require('@/assets/advisors/' + item.img)"
              class="w-100 h-100min"
            />
          </div>
        </div>
        <div class="w-80-S w-100-XS mx-5-S">
          <div
            class="w-100 fs-8-M fs-10-S fs-25-XS fw-600 ta-l pt-0-S pt-10-XS f-white-200"
          >
            {{ item.name }}
          </div>
          <div
            class="w-100 fs-6-M fs-8-S fs-20-XS fw-600 ta-l pb-2-S pb-5-XS pt-0-S pt-10-XS f-mcolor-100 tt-u"
          >
            {{ item.position }}
          </div>
          <div
            class="w-100 fs-5-M fs-8-S fs-20-XS ta-l pt-0-S pt-10-XS f-white-200 px-10-XS f-lh-15-S f-lh-45-XS"
          >
            <ul v-for="(list, m) in item.text" :key="m">
              <li>{{ list }}</li>
            </ul>
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
          img: "advisor1.png",
          logo: "nasa-logo.png",
          name: "Dr. Jong H. Baik",
          position: "Director of Hydrogen Technology",
          text: [
            "Liquid hydrogen technology expert with 25+ years of R&D experience",
            "Working with the US / international laboratories & government energy and space agencies",
            "Intensive technology evaluation on hydrogen value-chain companies including production, transfer storage for ground, aerial, sea and space application",
          ],
        },
        //  {
        //   img: "advisor2.png",
        //   logo: "nasa-logo.png",
        //   name: "Dr. William Notardonato",
        //   position: "Technical Advisor",
        //   text: [
        //     "The Founder and CEO of Eta Space LLC in Florida, The USA",
        //     "Chief Engineer and Cryogenic Fuel System Manager at NASA Kennedy Space Center",
        //     "An IAS (Institute of Advanced Studies) Western Australia University Fellow Professor",
        //     "A World Class  Engineer in Liquid Hydrogen and Oxygen Management",
        //   ],
        // },
        {
          img: "david.jpeg",
          name: "David Eunsung So",
          position: "Chief Executive Officer",
          text: [
            "Marketing Specialist & Business Developer with 20 years of experience in the U.S. & Korea",
            "An expert of R&D Coordinator, Tech and Market Trend Analysis",
            "Founding Member & CEO of Hydrogen Energy Company, H2Prime Inc.",
            "A Member of Hydrogen Energy Ambassador Council",
          ],
        },
        {
          img: "advisor3.jpeg",
          name: "Jonas Jonghyeon Kim",
          position: "Director of Strategy",
          text: [
            "Ananda Nirvana Kapital, Partner",
            "Das-Kapital(HG Ventures), Partner",
            "Fortune Korea, Europe Correspondent",
            "Atomrigs Lab, Marketer & BD",
          ],
        },
        // {
        //   img: "paul.png",
        //   name: "Paul Sandhu",
        //   position: "Director of Finance & Compliance",
        //   text: [
        //     "Chief Director of Prometheus LLC. in Hong Kong",
        //     "University of British Columbia Theoretical Physics Majored ",
        //     "Multi-Asset Quant Solutions & Client Advisory Head  MAQS",
        //     "Asia Pacific for BNP Paribas Asset Management  Board Member",
        //   ],
        // },
        {
          img: "user.png",
          name: "Preeyash Pradhan",
          position: "Director of Block-Chain Technology",
          text: ["Full-stack and Blockchain Engineer with 5+ years experience"],
        },
       
      ],
    };
  },
};
</script>
<style lang="css" scoped>
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

.my-logo-align {
  top: -5px;
  left: -25px;
}
</style>
