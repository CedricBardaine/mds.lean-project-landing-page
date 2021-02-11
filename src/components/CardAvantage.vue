<template>
  <div class="card-advantage">
    <div class="icon-container">
      <v-icon class="icon" style="font-size: 32px"> {{ icon }} </v-icon>
    </div>
    <h3 class="c-title">{{ title }}</h3>
    <div class="c-content">{{ content }}</div>
  </div>
</template>

<script>
export default {
  props: {
    icon: String,
    title: String,
    content: String
  }
};
</script>
