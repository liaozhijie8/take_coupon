<template>
  <CouponTake></CouponTake>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import CouponTake from '@/components/CouponTake.vue'

export default defineComponent({
  name: 'HomeView',
  components: {
    CouponTake
  }
})
</script>
