<template>
  <div id="app">
    <div class="bg-gray-200 min-h-screen p-8 flex items-center justify-center">
      <PropertyCard :property="property"/>
    </div>
  </div>
</template>

<script>
import PropertyCard from './components/PropertyCard'

export default {
  name: 'app',
  components: {
    PropertyCard
  },
  data: () => ({
    property: {
      imageUrl: './img/home.jpg',
      imageAlt: 'Rear view of modern home with pool',
      beds: 3,
      baths: 2,
      title: "Modern home in city center",
      priceInCents: 190000,
      formattedPrice: "$1,900.00",
      reviewCount: 34,
      rating: 4,
    }
  })
}
</script>

<style src="./assets/tailwind.css"></style>
