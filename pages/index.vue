<template>
<div class="bg-gray-900 text-white font-sans">
  <!-- Header -->
  <header class="bg-black text-white py-6">
    <div class="container mx-auto text-center">
      <h1 class="text-4xl font-semibold">BRTA - Bangladesh Road Transport Authority</h1>
      <p class="text-lg">Ensuring Safe and Efficient Transportation</p>
    </div>
  </header>

  <!-- Vehicle Registration Fees -->
  <!-- Vehicle Registration Fees -->
  <div class="container mx-auto py-8">
    <h2 class="text-3xl font-semibold mb-6">Vehicle Registration Fees</h2>

    <!-- Fees Table -->
    <table class="w-full border border-white rounded">
      <thead>
        <tr class="bg-gray-800 text-white">
          <th class="p-4">Vehicle Type</th>
          <th class="p-4">Registration Fee</th>
          <th class="p-4">Renewal Fee</th>
        </tr>
      </thead>
      <tbody>
        <!-- Fee Category 1 -->
        <tr class="bg-gray-700">
          <td class="p-4">Car</td>
          <td class="p-4">BDT 10,000</td>
          <td class="p-4">BDT 5,000</td>
        </tr>

        <!-- Fee Category 2 -->
        <tr class="bg-gray-700">
          <td class="p-4">Motorcycle</td>
          <td class="p-4">BDT 5,000</td>
          <td class="p-4">BDT 2,500</td>
        </tr>

        <!-- Fee Category 3 -->
        <tr class="bg-gray-700">
          <td class="p-4">Truck</td>
          <td class="p-4">BDT 15,000</td>
          <td class="p-4">BDT 7,500</td>
        </tr>
        <!-- Add more fee categories as needed -->
      </tbody>
    </table>
  </div>

  <!-- Latest News -->
  <div class="container mx-auto py-8">
    <h2 class="text-3xl font-semibold mb-6">Latest News</h2>

    <!-- News Articles with Animation -->
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
      <div class="bg-gray-800 p-6 border border-white rounded news-item">
        <h3 class="text-xl font-semibold mb-4">New Traffic Regulations</h3>
        <p class="text-gray-300">Stay updated on the latest traffic regulations to ensure a smooth driving experience.</p>
      </div>
      <div class="bg-gray-800 p-6 border border-white rounded news-item">
        <h3 class="text-xl font-semibold mb-4">Road Safety Awareness Campaign</h3>
        <p class="text-gray-300">Join us in promoting road safety through our awareness campaign. Your safety is our priority.</p>
      </div>
      <div class="bg-gray-800 p-6 border border-white rounded news-item">
        <h3 class="text-xl font-semibold mb-4">New Public Transport Guidelines</h3>
        <p class="text-gray-300">Learn about the updated guidelines for public transport to ensure a safe and comfortable journey.</p>
      </div>
      <div class="bg-gray-800 p-6 border border-white rounded news-item">
        <h3 class="text-xl font-semibold mb-4">Traffic Management Workshop</h3>
        <p class="text-gray-300">Participate in our upcoming workshop to contribute to effective traffic management in the city.</p>
      </div>
      <!-- Add more news articles as needed -->
    </div>
  </div>

  <!-- Additional Features -->
  <div class="container mx-auto py-8">
    <h2 class="text-3xl font-semibold mb-6">Additional Features</h2>

    <!-- Features Grid -->
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
      <!-- Feature 1 -->
      <div class="bg-gray-800 p-6 border border-white rounded">
        <h3 class="text-xl font-semibold mb-4">Online License Renewal</h3>
        <p class="text-gray-300">Renew your driver's license conveniently online. Save time and avoid queues.</p>
      </div>

      <!-- Feature 2 -->
      <div class="bg-gray-800 p-6 border border-white rounded">
        <h3 class="text-xl font-semibold mb-4">Traffic Updates</h3>
        <p class="text-gray-300">Receive real-time traffic updates and plan your journey accordingly.</p>
      </div>

      <!-- Feature 3 -->
      <div class="bg-gray-800 p-6 border border-white rounded">
        <h3 class="text-xl font-semibold mb-4">Educational Programs</h3>
        <p class="text-gray-300">Participate in our educational programs to enhance your knowledge of road safety.</p>
      </div>
      <!-- Add more features as needed -->
    </div>
    <footer class="bg-black py-4 mt-8">
    <div class="container mx-auto text-center">
      <!-- Add your footer content here -->
      <p class="text-gray-500">&copy; 2023 BRTA - Bangladesh Road Transport Authority. All rights reserved.</p>
    </div>
  </footer>
  </div>
</div>
</template>
  
<script>
</script>
  
<style scoped>
    @keyframes fadeIn {
      0% {opacity: 0.001}
      100% {opacity: 1}
    }

    .news-item {
      animation: fadeIn 1s ease-in-out;
    }
</style>
  