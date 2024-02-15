<template>
    <div class="w-100 home-bg home-bg-XS h-100min">
      <!-- <div class="w-100 h-100min p-f l-0 t-0 ovh-y-a bg-l" /> -->
      <Menu @connect="setModalFunc" :publicKey="publicKey" @logout="logout" />
      <Nuxt />
      <Footer />
      <!-- <AmModal
        :show="modal === 'connect'"
        :shadow="errorConnect ? 'shadow-red-100' : 'shadow-cyan-300'"
        max="w-fix-250-S w-90-XS"
        @closed="setModalFunc"
      >
        <ConnectWallet
          @cancel="setModalFunc"
          @set="connectWalletFunc"
          :wallets="wallets"
          :error="errorConnect"
          :loader="loaderConnect"
        />
      </AmModal>
      <AmModal
        :show="modal === 'connectError'"
        shadow="shadow-red-100"
        max="w-fix-250-S w-90-XS"
        @closed="setModalFunc"
      >
        <ConnectError />
      </AmModal> -->
    </div>
  </template>
  
  <script>
  import Menu from "@/components/Menu";
  import Footer from "@/components/Footer";
  
  export default {
    components: {
      Menu,
      Footer,
    },
  };
  </script>
  
  <style>
    
  </style>