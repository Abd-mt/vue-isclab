<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template >
  <div class="greetings" backgraund="aqua">
    <h1 class="green" >{{ msg }}</h1>
    <h3>
      Laboratorio de sistemas y aplicaciones web
      <a href="contacto@isclab.com.mx" target="_blank" rel="noopener">contacto@isclab.com.mx</a> 
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}
background{
  background-color: aqua;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>