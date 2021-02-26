<template>
  <div>
    <div class="text-gray-600">
      <header class="mb-5">
        <div class="bg-gray-700 p-4 text-white">Helo world.</div>
      </header>
      <main class="container mx-auto">
        <div class="text-center text-5xl">我也為此而來！</div>
        <hr />
        <div class="text-komabig">雪莉大字體</div>
        <div class="my-5 bg-bootstrap_primary text-white">
          你剛剛攻打我的村莊！？
        </div>
        <div class="my-5 bg-bootstrap_success text-white">
          你剛剛攻打我的村莊！？
        </div>
        <div class="my-5 bg-bootstrap_danger text-white">
          你剛剛攻打我的村莊！？
        </div>
        <!-- 循环各种字号 Start -->
        <ul>
          <li v-for="(fontsize, i) in list" :key="i">
            <div :class="fontsize">Tailwind CSS</div>
          </li>
        </ul>
        <!-- 循环各种字号 End -->
        <hr class="my-5" />
        <div class="flex justify-center">
          <img
            src="https://raw.githubusercontent.com/komavideo/LearnTailwindCSS/main/tailwindcss.png"
            class="shadow-lg border my-5"
          />
        </div>
      </main>
      <footer class="mt-5">
        <div class="bg-gray-300 p-4 text-black">你好，Tailwind CSS。</div>
      </footer>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      list: [
        "text-xs",
        "text-sm",
        "text-base",
        "text-lg",
        "text-xl",
        "text-2xl",
        "text-3xl",
        "text-4xl",
        "text-5xl",
        "text-6xl",
        "text-7xl",
        "text-8xl",
        "text-9xl"
      ]
    };
  }
};
</script>
