<!-- SPDX-License-Identifier: AGPL-3.0-or-later -->
<template>
  <CardSearchResult
    :user="user"
    :isReduced="isReduced"
    :isPrivate="isPrivate"
  />
</template>

<script setup lang="ts">
import type { User } from "~/types/auth/user";

defineProps<{
  user: User;
  isPrivate?: boolean;
  isReduced?: boolean;
}>();
</script>
