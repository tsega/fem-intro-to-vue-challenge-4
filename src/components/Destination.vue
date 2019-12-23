<template>
  <div class="destination">
    <img :src="location.img" />
    <h2>{{location.name}}</h2>
    <p>{{location.desc}}</p>
  </div>
</template>

<script>
export default {
  name: 'Destination',
  props: ['location']
}
</script>

<style lang="scss" scoped>
.destination {
  display: flex;
  flex-direction: column;
  width: 280px;
  height: 320px;
  justify-content: center;
  background: white;
  border: 1px solid #ddd;
  padding: 20px 20px;
  margin: 10px;
  h2 {
    margin: 0;
    text-align: center;
  }
  img {
    margin: 10px;
    align-self: center;
  }
  p {
    line-height: 1;
  }
}
</style>
