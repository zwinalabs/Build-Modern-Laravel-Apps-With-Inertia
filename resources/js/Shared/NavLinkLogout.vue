
<template>
  <Link
    class="text-blue-500 hover:underline" method="post" as="button">
    <slot />
  </Link>
    
</template>
<script>
import { Link } from "@inertiajs/inertia-vue3";

export default {
  components: { Link },
};
</script>