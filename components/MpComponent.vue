<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      names: ["toto", "tete", "Titi"]
    };
  },
  props: {
    tag: String
  },
  render(createElement) {
    return createElement("div", {}, [
      createElement("form", { attrs: { method: "POST" } }, [
        createElement("script", {
          attrs: {
            src:
              "https://www.mercadopago.com.ar/integrations/v1/web-payment-checkout.js"
          }
        })
      ])
    ]);

    //   <form method="POST" ref="mpBtn" id="mpBtn">
    //   <script
    // src="https://www.mercadopago.com.ar/integrations/v1/web-payment-checkout.js"
    // data-preference-id="654853549-4154ee41-3993-432a-a273-a45a9c23c559"
    // data-header-color="#e8e6d6"
    // data-elements-color="#e8e6d6"
    // data-button-label="PAGAR"
    //   ><\/script>
    // </form>
  }
};
</script>

<style></style>
