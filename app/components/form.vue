<template>
    <form class="w-full max-w-md mx-auto space-y-6">
  <!-- Form Header -->
  <div class="text-center">
    <h2 class="text-2xl font-bold text-gray-800">Join Our Movement</h2>
  </div>

  <!-- Full Name -->
  <div class="space-y-2">
    <label for="fullName" class="block text-md font-medium text-gray-700">Full Name</label>
    <input 
      type="text" 
      id="fullName" 
      name="fullName" 
      placeholder="Enter your full name" 
      required
      class="w-full px-4 py-2 border border-gray-300 rounded-md focus:ring-2 focus:ring-blue-500 focus:border-blue-500"
    >
  </div>

  <!-- Email -->
  <div class="space-y-2">
    <label for="email" class="block text-md font-medium text-gray-700">Email Address</label>
    <input 
      type="email" 
      id="email" 
      name="email" 
      placeholder="Enter your email" 
      required
      class="w-full px-4 py-2 border border-gray-300 rounded-md focus:ring-2 focus:ring-blue-500 focus:border-blue-500"
    >
  </div>

  <!-- Phone -->
  <div class="space-y-2">
    <label for="phone" class="block text-md font-medium text-gray-700">Phone Number</label>
    <input 
      type="tel" 
      id="phone" 
      name="phone" 
      placeholder="Enter your phone number"
      class="w-full px-4 py-2 border border-gray-300 rounded-md focus:ring-2 focus:ring-blue-500 focus:border-blue-500"
    >
  </div>

  <!-- Location -->
 
  <!-- Contribution -->
  <div class="space-y-2">
    <label class="block text-md font-medium text-gray-700">How would you like to contribute?</label>
    <div class="grid grid-cols-2 gap-2">
      <label class="flex items-center space-x-2">
        <input type="checkbox" name="contribute" value="volunteer" class="rounded text-blue-600 focus:ring-blue-500">
        <span class="text-sm text-gray-700">Volunteer</span>
      </label>
      <label class="flex items-center space-x-2">
        <input type="checkbox" name="contribute" value="donate" class="rounded text-blue-600 focus:ring-blue-500">
        <span class="text-sm text-gray-700">Donate</span>
      </label>
      <label class="flex items-center space-x-2">
        <input type="checkbox" name="contribute" value="organize" class="rounded text-blue-600 focus:ring-blue-500">
        <span class="text-sm text-gray-700">Organize Events</span>
      </label>
      <label class="flex items-center space-x-2">
        <input type="checkbox" name="contribute" value="spread" class="rounded text-blue-600 focus:ring-blue-500">
        <span class="text-sm text-gray-700">Spread Awareness</span>
      </label>
    </div>
  </div>

  
  <button 
    type="submit" 
    class="w-full px-6 py-3 bg-blue-600 text-white font-medium rounded-md hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-blue-500 focus:ring-offset-2 transition-colors"
  >
    Register for the Movement
  </button>
</form>
</template>