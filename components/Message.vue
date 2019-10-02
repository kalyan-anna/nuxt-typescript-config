<template>
  <div>
    Name: {{ fullName }}
    Message: {{ message }}
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "nuxt-property-decorator";

interface User {
  firstName: string;
  lastName: number;
}

@Component
export default class Message extends Vue {
  message: string = "This is a message";

  get fullName(): string {
    return "Ful name Kalyan...";
  }
}
</script>
