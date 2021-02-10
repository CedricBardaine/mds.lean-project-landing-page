<template>
  <v-card
    class=""
    color="#5139ea"
    dark
    rounded
    style="max-width: 433px; min-height:540px; padding: 45px; border-radius: 51px !important"
  >
    <v-col align="" class="pa-4">
      <v-row class="pt-2 pb-10">
        <v-btn class="custom-roundedIcon" fab :ripple="false">
          <v-icon color="#5139ea"> {{ icon }} </v-icon>
        </v-btn>
      </v-row>
      <v-row class="pt-2 pb-10"
        ><h3>{{ title }}</h3></v-row
      >
      <v-row class="pt-2 pb-2">{{ content }}</v-row>
    </v-col>
  </v-card>
</template>

<script>
export default {
  props: {
    icon: String,
    title: String,
    content: String,
  },
};
</script>