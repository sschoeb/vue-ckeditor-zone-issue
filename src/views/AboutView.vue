
<script setup lang="ts">
import CKE from "@ckeditor/ckeditor5-vue";
const CKEditor = CKE.component;

import ClassicEditor from "@ckeditor/ckeditor5-build-classic";

const config = {};

</script>

<template>
  <div class="about">
    <h1>This is an about page</h1>
      <CKEditor
              :editor="ClassicEditor"
              :config="config"
      ></CKEditor>
    </div>

</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
