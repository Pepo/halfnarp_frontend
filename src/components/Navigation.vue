<style lang="scss" scoped>
 .navigation {
     background-color: #7F7F7F;
 }
 .navigation__inner-wrapper {
     max-width: 1280px;
     margin: 0 auto;
     padding: 0.5rem;
     display: flex;
     flex-wrap: wrap;
     align-items: baseline;
 }
 .navigation__button {
     border: none;
     padding: 0.2rem 0.5rem;
     font-size: 1rem;
     margin: 0.5rem;
     background-color: #000;
     color: #FFF;
 }
 .navigation__headline {
     color: #FFF;
     font-size: 1rem;
 }
</style>

<template>
	<nav class="navigation">
        <div class="navigation__inner-wrapper">
            <h2 class="navigation__headline">Filter:</h2>
            <button class="navigation__button">CCC</button>
            <button class="navigation__button">Art + Culture</button>
            <button class="navigation__button">Ethics, Politics + Society</button>
            <button class="navigation__button">Hardware</button>
            <button class="navigation__button">Resilience</button>
            <button class="navigation__button">Science</button>
            <button class="navigation__button">Security</button>
            <button class="navigation__button">Entertainment</button>

        </div>
	</nav>
</template>

<script>
export default {
  name: 'Navigation'
}
</script>
