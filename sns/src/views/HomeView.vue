<template>
  <div class="home-container bg-gradient-to-br from-bright-pink via-bright-purple to-bright-yellow min-h-screen flex flex-col items-center justify-center">
    <div class="max-w-4xl bg-white rounded-lg shadow-2xl p-8 text-center">
      <h1 class="text-5xl font-bold mb-4 text-bright-gradient">Welcome to AceBook!</h1>
      <p class="text-lg text-gray-800 font-medium mb-6">
        Dive into a vibrant community where you can connect, share, and shine!
      </p>
      <div class="flex justify-center space-x-6">
        <router-link
          to="/signup"
          class="px-8 py-3 bg-bright-blue text-white font-semibold rounded-full shadow-lg transform hover:scale-105 transition-transform"
        >
          Sign Up
        </router-link>
        <router-link
          to="/login"
          class="px-8 py-3 bg-bright-green text-white font-semibold rounded-full shadow-lg transform hover:scale-105 transition-transform"
        >
          Log In
        </router-link>
      </div>
    </div>
    <div class="mt-8">
      <img
        src="https://i.pravatar.cc/301"
        alt="Community Illustration"
        class="w-full max-w-md rounded-lg shadow-lg"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeView",
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap');

.home-container {
  font-family: 'Poppins', sans-serif;
}

.text-bright-gradient {
  background: linear-gradient(to right, #ff007a, #a700ff, #ffb900);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

/* Bright color palette */
.bg-bright-pink {
  background-color: #ff007a;
}

.bg-bright-purple {
  background-color: #a700ff;
}

.bg-bright-yellow {
  background-color: #ffb900;
}

.bg-bright-blue {
  background-color: #007bff;
}

.bg-bright-green {
  background-color: #28a745;
}

.bg-gradient-to-br {
  background: linear-gradient(to bottom right, #ff007a, #a700ff, #ffb900);
}

/* Buttons */
.router-link {
  transition: transform 0.3s ease-in-out;
}
</style>
