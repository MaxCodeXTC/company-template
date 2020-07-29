<template>
  <div class="flex flex-col h-screen w-screen">
    <!--
      Navigation Bar

      PARAMETERS
      :logoURL  (URL for Logo)
    -->
    <NaviWrapper
      imgURL="https://www.logolynx.com/images/logolynx/99/99ea79e039ed844020667ed3ed9f1544.png"
    ></NaviWrapper>

    <div class="flex-1">
      <div class="flex">
        <Nuxt class="w-full h-screen overflow-y-auto"/>
      </div>
    </div>
    <FooterWrapper/>
  </div>
</template>
<script>
export default {};
</script>