<template>
  <footer>
    <div class="flex flex-col items-center mt-16">
      <div class="flex mb-3 space-x-4">
        <a
          class="text-sm text-gray-500 transition hover:text-gray-600"
          target="_blank"
          rel="noopener noreferrer"
          :href="siteMetadata.github"
          ><span class="sr-only">github</span>
          <img class="w-8 h-8" src="~assets/icon/github_new.svg" /> </a
        ><a
          class="text-sm text-gray-500 transition hover:text-gray-600"
          target="_blank"
          rel="noopener noreferrer"
          :href="siteMetadata.linkedin"
          ><span class="sr-only">Linkedin</span>
          <img class="w-8 h-8" src="~assets/icon/linkeding.svg" /> </a
        ><a
          class="text-sm text-gray-500 transition hover:text-gray-600"
          target="_blank"
          rel="noopener noreferrer"
          :href="`mailto:${siteMetadata.email}`"
          ><span class="sr-only">mail</span>
          <img class="w-8 h-8" src="~assets/icon/mail.svg" /></a
        ><a
          class="text-sm text-gray-500 transition hover:text-gray-600"
          target="_blank"
          rel="noopener noreferrer"
          :href="siteMetadata.facebook"
          ><span class="sr-only">facebook</span>
          <img class="w-8 h-8" src="~assets/icon/facebook.svg"
        /></a>
        <a
          class="text-sm text-gray-500 transition hover:text-gray-600"
          target="_blank"
          rel="noopener noreferrer"
          :href="siteMetadata.youtube"
          ><span class="sr-only">youtube</span>
          <img class="w-8 h-8" src="~assets/icon/youtube.svg"
        /></a>
      </div>
      <div class="flex mb-2 space-x-2 text-sm text-gray-500 dark:text-gray-400">
        <div>
          © Copyright {{ new Date().getFullYear() }} ※本站採用
          <a href="https://creativecommons.org/licenses/by-nc-sa/3.0/tw/">CC授權</a>
          歡迎引用與介紹，並註明出處，謝謝
        </div>
      </div>
      <div class="mb-8 text-sm text-gray-500 dark:text-gray-400">
        <a
          target="_blank"
          rel="noopener noreferrer"
          href="https://github.com/mdrathik/tailwind-nuxtjs-starter-blog"
        ></a>
      </div>
    </div>
  </footer>
</template>

<script>
import siteMetaInfo from "@/data/sitemetainfo";
export default {
  data() {
    return {
      siteMetadata: siteMetaInfo,
    };
  },
};
</script>
