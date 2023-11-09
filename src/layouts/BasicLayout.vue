<template>
  <div id="basicLayout">
    <a-layout style="height: 400px">
      <a-layout-header class="header">
        <GlobalHeader />
      </a-layout-header>
      <a-layout-content class="content">
        <router-view />
      </a-layout-content>
      <a-layout-footer class="footer">Voj by Victor</a-layout-footer>
    </a-layout>
  </div>

  <router-view />
</template>

<style scoped>
#basicLayout {
}

#basicLayout .header {
  background: red;
  margin-bottom: 16px;
}

#basicLayout .content {
  background: linear-gradient(to right, #bbb, #fff);
  margin-bottom: 16px;
}

#basicLayout .footer {
  background: #efefef;
  padding: 16px;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  text-align: center;
}
</style>
<script setup lang="ts">
import GlobalHeader from "@/components/GlobalHeader.vue";
</script>
