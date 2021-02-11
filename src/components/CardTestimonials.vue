<template >
  <v-card
    dark
    rounded
    style="
      min-width: 436px;
      min-height: 492px;
      padding: 24px 32px;
      border-radius: 51px !important;
      background-color: white;
      color: black;
      margin-right: 71px;
    "
  >
    <v-img
      :src="img ? img : 'https://cataas.com/cat/says/hello'"
      style="width: 163px; height: 163px; border-radius: 100%"
    ></v-img>
    <h3 style="padding-top: 60px; padding-bottom: 23px">
      {{ name ? name : "Jean Dujardin" }}
    </h3>
    <p style="max-width: 307px">
      {{ content ? content : defaultContent }}
    </p>

    <img
      src="../assets/img/Vector.svg"
      alt='"'
      style="position: absolute; top: -1px; right: -1px"
    />
    <img
      src="../assets/img/Vector.svg"
      alt='"'
      style="position: absolute; top: -1px; right: 85px"
    />
  </v-card>
</template>
<script>
export default {
  props: {
    img: String,
    name: String,
    content: String,
  },
  data: () => ({
    defaultContent:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nibh tellus nec ut at tortor, velit urna viverra nibh. Dui morbi ultrices eros adipiscing viverra accumsan, ipsum nunc sed.",
  }),
};
</script>
<style lang="">
</style>