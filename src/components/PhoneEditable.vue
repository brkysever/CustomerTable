<template>
  <div>
    <p v-if="!isEditMode" @click="isEditMode = true">{{ phone || "-" }}</p>
    <input v-model="newPhone" @blur="changePhone" v-else autofocus />
  </div>
</template>

<script>
export default {
  name: "PhoneEditable",
  props: ["phone"],
  data() {
    return {
      isEditMode: false,
      newPhone: this.phone,
    };
  },
  methods: {
    changePhone() {
      this.isEditMode = false;
      this.$emit("phone-changed", this.newPhone);
    },
  },
};
</script>

<style></style>
