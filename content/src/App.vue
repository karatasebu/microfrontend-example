<template>
  <div ref="root"></div>
  <div class="content">
    <h3 class="title">VUE CONTENT</h3>
    <p class="text">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam dolore
      fugiat mollitia asperiores, ea libero quos laboriosam, tempore illo odit
      deserunt hic dignissimos tenetur voluptatum vel totam eum ex? Hic. Lorem
      ipsum dolor sit amet, consectetur adipisicing elit. Veritatis a assumenda
      libero in explicabo quisquam fuga reprehenderit, qui, nam aliquid nostrum,
      incidunt rem tempora modi molestiae accusamus quae praesentium aliquam.
      Lorem ipsum, dolor sit amet consectetur adipisicing elit. Iste itaque,
      accusantium sint nam maiores ullam excepturi. Omnis eligendi nisi minima
      praesentium, eius labore culpa similique blanditiis? Voluptates numquam
      explicabo dolore.
    </p>
  </div>
</template>

<script setup>
import { ref, onMounted } from "vue";
import React from "react";
import ReactDOM from "react-dom";
import "./index.css";
import Header from "header/App";

const root = ref(null);

onMounted(() => {
  ReactDOM.render(React.createElement(Header), root.value);
});
</script>
