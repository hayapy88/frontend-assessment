<template>
  <div>
    <Hero />
    <Card />
  </div>
</template>

<script>
import Hero from "./components/Hero";
import Card from "./components/Card";

export default { name: "App", components: { Hero, Card } };
</script>
