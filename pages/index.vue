<template>
  <div
    class="flex h-screen"
    :class="color[rand]"
    @click="rand = Math.floor(Math.random() * 10)"
  >
    <div class="m-auto">
      <Logo />
      <h1 class="font-mono text-6xl text-gray-800 text-center">ST104</h1>
      <div class="text-center">
        <a
          href="http://www.sattha.ac.th/2017/"
          target="_blank"
          rel="noopener noreferrer"
        >
          <button
            class="text-base font-medium rounded-lg p-3 mx-2 bg-green-500 text-white transition duration-300 ease-in-out transform hover:scale-125"
          >
            Website
          </button>
        </a>
        <a
          href="https://github.com/BlackBird-Coding/Nuxt-ST104"
          target="_blank"
          rel="noopener noreferrer"
        >
          <button
            class="text-base font-medium rounded-lg p-3 mx-2 bg-gray-700 text-white transition duration-300 ease-in-out transform hover:scale-125"
          >
            GitHub
          </button>
        </a>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      color: [
        'bg-white',
        'bg-red-300',
        'bg-yellow-300',
        'bg-green-300',
        'bg-blue-300',
        'bg-indigo-300',
        'bg-purple-300',
        'bg-pink-300',
        'bg-gray-300',
      ],
      rand: 0,
    }
  },
}
</script>
