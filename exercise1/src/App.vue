<template>
  <div>
    <Hero />
    <Card />
  </div>
</template>

<script>
import HeroSection from "./components/sections/HeroSection";
import CardSection from "./components/sections/CardSection";
import Card from "./components/ui/Card";
import Button from "./components/ui/Button";

export default { name: "App", components: { Hero, Card } };
</script>
