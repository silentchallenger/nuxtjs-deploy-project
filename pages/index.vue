<script setup>
useHead({
  title: "Home Page"
});
const cards = [
  {
    info: {
      title: "Accessible Front-end Components",
      description:
        "Reliable accessible UI components: :focus styles, modals, date pickers, navigation, tables, buttons, SVGs.",
    },
    link: {
      url: "https://www.smashingmagazine.com/2021/03/complete-guide-accessible-front-end-components/",
      text: "Explore Accessible Components",
    },
    colors: {
      bgLight: "bg-green-100",
      bgDark: "bg-green-600",
      textDark: "text-green-600",
    },
  },
  {
    info: {
      title: "CSS Generators & Tools",
      description:
        "Reliable accessible UI components: :focus styles, modals, date pickers, navigation, tables, buttons, SVGs.",
    },
    link: {
      url: "https://www.smashingmagazine.com/2021/03/complete-guide-accessible-front-end-components/",
      text: "Explore Accessible Components",
    },
    colors: {
      bgLight: "bg-orange-100",
      bgDark: "bg-orange-600",
      textDark: "text-orange-600",
    },
  },
  {
    info: {
      title: "Frontend Boilerplate and Starter Kits",
      description:
        "Reliable accessible UI components: :focus styles, modals, date pickers, navigation, tables, buttons, SVGs.",
    },
    link: {
      url: "https://www.smashingmagazine.com/2021/03/complete-guide-accessible-front-end-components/",
      text: "Explore Accessible Components",
    },
    colors: {
      bgLight: "bg-purple-100",
      bgDark: "bg-purple-600",
      textDark: "text-purple-600",
    },
  },
];
</script>

<template>
  <AppMain>
    <AppHeader pageTitle="Home Page" />
    <section>
      <header class="text-3xl text-center py-4 font-semibold">
        <h2>Cards</h2>
      </header>
      <AppCard
        v-for="card in cards"
        :key="card.id"
        :info="card.info"
        :link="card.link"
        :colors="card.colors" />
    </section>
  </AppMain>
</template>