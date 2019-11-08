<template>
  <Layout>
    <main role="main">
      <section class="hero">
        <div class="hero__contentWrapper">
          <p class="hero__lead">Hello</p>
          <h2 class="hero__title">It's Paul</h2>
          <p class="hero__desc">The Front End Developer you need!</p>
        </div>

        <div class="hero__socialIcons socialIcons">
          <a href="#" class="socialIcons_link">
            <font-awesome class="socialIcons__icon" :icon="['fab', 'github']" />
          </a>
          <a href="#" class="socialIcons_link">
            <font-awesome class="socialIcons__icon" :icon="['fab', 'linkedin']" />
          </a>
        </div>

        <div class="hero__scrollBtn">
          <font-awesome :icon="['fas', 'arrow-down']" />
        </div>
      </section>
    </main>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "Ozi Ocb Portfolio"
  }
};
</script>

<style lang="scss">
.hero {
  background-color: #900;
  height: 100vh;
  display: grid;
  // TODO: Add the Grid
}
</style>
