<script setup>
import HelloWorld from './components/HelloWorld.vue';
import TheWelcome from './components/TheWelcome.vue';
</script>

<template>
    <header>
        <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

        <p class="classe">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptate dignissimos facilis quod
            reprehenderit sit, ea animi, fugiat vel voluptatum recusandae esse consequatur possimus repudiandae quaerat
            architecto dicta ipsum perferendis inventore.</p>
        <div class="wrapper">
            <HelloWorld msg="You did it!" />
        </div>
    </header>


    <main>
        <TheWelcome />
    </main>
</template>


<style scoped>
.classe {
    color: red;
}

header {
    line-height: 1.5;
}

.logo {
    display: block;
    margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
    header {
        display: flex;
        place-items: center;
        padding-right: calc(var(--section-gap) / 2);
    }

    .logo {
        margin: 0 2rem 0 0;
    }

    header .wrapper {
        display: flex;
        place-items: flex-start;
        flex-wrap: wrap;
    }
}
</style>

<!-- <style scoped lang="sass">
header
  line-height: 1.5
  background-color: lightblue

  .classe
    color: red

  @media (min-width: 1024px)
    display: flex
    place-items: center
    padding-right: calc(var(--section-gap) / 2)

    .wrapper
      display: flex
      place-items: flex-start
      flex-wrap: wrap

.logo
  display: block
  margin: 0 auto 2rem
  @media (min-width: 1024px)
    margin: 0 2rem 0 0
</style> -->
