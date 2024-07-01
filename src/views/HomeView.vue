<template>
  <div class="home">
    Home
    <p>My name is {{ name }} and age is {{ age }}</p>
    <button @click="handleClick">Click</button>
  </div>
</template>

<script>
export default {
  name: 'HomeView',
  setup() {
    let name = 'mario'
    let age = 30

    const handleClick = () => {
      console.log('clicked')
    }

    return {
      name, age, handleClick
    }
  }
}
</script>
