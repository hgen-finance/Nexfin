<template>
  <div class="container pt-0-L pt-0-M pt-10-S pt-40-XS">
    <div
      class="w-100 f-white-200 tt-u fs-14-S fs-25-XS fw-600 ta-c px-10-XS fd-r jc-c ai-c"
    >
      <!-- <img
        src="@/assets/svg/company_logo.png"
        class="h-fix-20-M h-fix-30-S h-fix-55-XS mr-2-M mr-3-S mr-3-XS"
      /> -->
      <!-- <img
        src="@/assets/svg/nexfin-logo.png"
        class=" h-fix-10-M h-fix-15-S h-fix-30-XS mr-2 ml-5-XS"
      /> -->
      <div
        class="w-100-S w-100-XS fd-r fs-12-S fs-25-XS f-white-200 fw-600 ai-c jc-c"
      >
        <img
          src="@/assets/svg/symbol-hgen.png"
          class="h-fix-20-S h-fix-20-S h-fix-35-XS mr-2-S mr-5-XS"
        />
        $HGEN
      </div>
    </div>
    <div
      class="w-100 gradient tt-u fs-20-S fs-25-XS fw-900 ta-c pt-4-S pt-15-XS"
    >
      $ {{ getTotal }}
    </div>
    <div class="w-100 f-gray-400 ta-c fs-6-S fs-15-XS fw-500">
      Total Deposited Value
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      mobile: false,
    };
  },
  props: {
    publicKey: { type: String, default: null },
  },
  computed: {
    getTotal() {
      let res = "000000000000";
      const total =0;
      if (total) {
        res = res.substr(0, res.length - total.toString().length) + total;
      }
      return res.toString().replace(/(.)(?=(\d{3})+$)/g, "$1,");
    },
  },
};
</script>
