<template>
  <Page>
    <ActionBar title="Stract2" />
    <FlexboxLayout flexDirection="column">
      <Label class="message" :text="`${msg} ${counter}`" height="100" />
      <Button text="Button" @tap="counter += 1" height="100" />
    </FlexboxLayout>
  </Page>
</template>

<script lang="ts">
export default {
  data() {
    return {
      msg: "Hello World!",
      counter: 0,
    };
  },
};
</script>

<style scoped>
ActionBar {
  background-color: #53ba82;
  color: #ffffff;
}

.message {
  vertical-align: center;
  text-align: center;
  font-size: 20;
  color: #333333;
}
</style>
