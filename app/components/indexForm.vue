<template>
    <section :class="['py-12 md:py-14 lg:py-16 font-[Uno] bg-[#FAFAFA]', light ? 'bg-gray-50' : 'bg-white'] ">
      <div class="container mx-auto px-4 md:px-6 lg:px-8">
        <!-- Section Header -->
        <div class="text-center mb-10 md:mb-12 lg:mb-14">
          <h2 class="text-3xl md:text-3xl lg:text-4xl font-bold text-gray-800 mb-3">
            {{ title }}
          </h2>
          <p class="text-base md:text-lg lg:text-xl text-gray-600 max-w-2xl mx-auto">
            {{ subtitle }}
          </p>
          <div class="mt-5">
            <div class="w-[70px] h-[3px] bg-[#BC361D] mx-auto rounded-full"></div>
            <div class="w-[35px] h-[3px] bg-[#BC361D] mx-auto mt-[3px] opacity-60 rounded-full"></div>
          </div>
        </div>
  
        <!-- Form Container -->
        <div class="w-full max-w-2xl mx-auto">
          <form class="w-full space-y-6 md:space-y-7">
            <!-- Full Name -->
            <div class="space-y-2">
              <label for="fullName" class="block text-base md:text-lg font-medium text-gray-700">Full Name</label>
              <input 
                type="text" 
                id="fullName" 
                name="fullName" 
                placeholder="Enter your full name" 
                required
                class="w-full px-4 py-3 text-base md:text-lg border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500"
              >
            </div>
  
            <!-- Email -->
            <div class="space-y-2">
              <label for="email" class="block text-base md:text-lg font-medium text-gray-700">Email Address</label>
              <input 
                type="email" 
                id="email" 
                name="email" 
                placeholder="Enter your email" 
                required
                class="w-full px-4 py-3 text-base md:text-lg border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500"
              >
            </div>
  
            <!-- Phone -->
            <div class="space-y-2">
              <label for="phone" class="block text-base md:text-lg font-medium text-gray-700">Phone Number</label>
              <input 
                type="tel" 
                id="phone" 
                name="phone" 
                placeholder="Enter your phone number"
                class="w-full px-4 py-3 text-base md:text-lg border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500"
              >
            </div>
  
            <!-- Contribution -->
            <div class="space-y-2">
              <label class="block text-base md:text-lg font-medium text-gray-700">How would you like to contribute?</label>
              <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                <label class="flex items-center space-x-3 p-3 border border-gray-200 rounded-lg hover:bg-gray-50">
                  <input type="checkbox" name="contribute" value="volunteer" class="w-5 h-5 rounded text-blue-600 focus:ring-blue-500">
                  <span class="text-base md:text-lg text-gray-700">Volunteer</span>
                </label>
                <label class="flex items-center space-x-3 p-3 border border-gray-200 rounded-lg hover:bg-gray-50">
                  <input type="checkbox" name="contribute" value="donate" class="w-5 h-5 rounded text-blue-600 focus:ring-blue-500">
                  <span class="text-base md:text-lg text-gray-700">Donate</span>
                </label>
                <label class="flex items-center space-x-3 p-3 border border-gray-200 rounded-lg hover:bg-gray-50">
                  <input type="checkbox" name="contribute" value="organize" class="w-5 h-5 rounded text-blue-600 focus:ring-blue-500">
                  <span class="text-base md:text-lg text-gray-700">Organize Events</span>
                </label>
                <label class="flex items-center space-x-3 p-3 border border-gray-200 rounded-lg hover:bg-gray-50">
                  <input type="checkbox" name="contribute" value="spread" class="w-5 h-5 rounded text-blue-600 focus:ring-blue-500">
                  <span class="text-base md:text-lg text-gray-700">Spread Awareness</span>
                </label>
              </div>
            </div>
  
            <!-- Submit Button -->
            <button 
              type="submit" 
              class="w-full px-6 py-3 bg-[#202654] text-white text-base md:text-lg font-medium rounded-lg hover:bg-blue-700 focus:outline-none focus:ring-4 focus:ring-blue-500 focus:ring-offset-2 transition-colors"
            >
              Register for the Movement
            </button>
          </form>
        </div>
      </div>
    </section>
  </template>
  
  
  <script>
  export default {
    name: 'FullWidthForm',
    props: {
      title: {
        type: String,
        default: "JOIN OUR MOVEMENT"
      },
      subtitle: {
        type: String,
        default: "We're building a movement to transform our nation's future"
      },
      light: {
        type: Boolean,
        default: true
      }
    }
  }
  </script>