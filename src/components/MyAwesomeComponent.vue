<template>
  <div>
    <button @click="incrementPension">Increment my pension</button>
    <p>Your pension will be: {{ pension }}</p>
  </div>
</template>

<script>
import { ref } from 'vue';

export default {
  name: "MyAwesomeComponent",
  setup() {
    const pension = ref(20);

    function incrementPension() {
      pension.value++;
    }

    return {
      pension, incrementPension
    };
  },
};
</script>
