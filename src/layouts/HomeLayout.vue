<template>
  <div>
    <div class="top banner">
      <slot name="primary">
      </slot>
    </div>
    <div class="middle banner">
      <slot name="secondary">
      </slot>
    </div>
    <div class="bottom banner">
      <slot name="contact">
      </slot>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeLayout",
};
</script>

<style scoped>
.banner {
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
  display: flex;
  width: 99vw;
  height: 98vh;
  margin: auto 0;
}

.top {
  padding: 20px;
  margin: 30px 10px 10px;
  overflow-x: hidden;
}

.middle {
  display: flex;
  flex-direction: row;
  background-color: #35abbb;
  padding: 20px;
  margin: 10px;
  overflow-x: hidden;
}

.bottom {
  background-color: #35ddee;
  margin: 10px;
  overflow-x: hidden;
}
</style>