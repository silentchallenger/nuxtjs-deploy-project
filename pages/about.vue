<script setup>
useHead({
  title: "About Page"
});
const cod = [
  {
    name: "Captain Price",
    description: "Cold-blooded commander"
  },
  {
    name: "Soap McTavish",
    description: "Rookie soldier"
  },
]
</script>
<template>
  <AppMain>
    <AppHeader pageTitle="About Page" />
    <div class="flex space-around gap-4 flex-wrap">
      <section>
        <h3>Unordered List</h3>
        <AppList bullets>
          <AppListItem v-for="item in cod" :key="item.id" brand>
            <h4>{{ item.name }}</h4>
            <p>{{ item.description }}</p>
          </AppListItem>
        </AppList>
      </section>
      <section>
        <h3>Ordered List</h3>
        <AppList ordered>
          <li>one</li>
          <li>two</li>
          <li>three</li>
        </AppList>
      </section>
    </div>
    <div>
      <nuxt-img 
        src="images/corgi.jpeg"
        sizes="sm:100vw md:80vw lg:50vw"
        loading="lazy"
        format="webp"
        class="mx-auto"
      />
    </div>
  </AppMain>
</template>