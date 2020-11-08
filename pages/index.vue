<template>
  <div>
    <h1>TEST MP BUTTON (NUXT)</h1>
    <form method="POST" ref="mpBtn" id="mpBtn" v-html="ishere"></form>
    <h2>^^^Button Should be Here^^^</h2>
  </div>
</template>

<script>
export default {
  data() {
    return {
      ishere: `<script
        v-if="ishere"
        src="https://www.mercadopago.com.ar/integrations/v1/web-payment-checkout.js"
        data-preference-id="654853549-4154ee41-3993-432a-a273-a45a9c23c559"
        data-header-color="#e8e6d6"
        data-elements-color="#e8e6d6"
        data-button-label="PAGAR"
      ><\/script>`
    };
  }
};
</script>
