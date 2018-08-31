<template>
  <footer class="max-w-2xl mx-auto px-5 md:px-10 py-8 text-theme-text-tertiary flex flex-col lg:flex-row flex-wrap justify-between items-center">
    <div class="mb-4 lg:mb-0">
      <span class="block md:inline-block mb-4 md:mb-0 text-center">&copy; CryptoMountains | {{ year }}. {{ $t("All rights reserved") }}</span></div>
    </div>
    <div class="text-center">
    </div>
  </footer>
</template>

<script type="text/ecmascript-6">
import moment from 'moment'

export default {
  computed: {
    year() {
      return moment().format('Y')
    },
    version() {
      return GIT_VERSION
    },
    versionLink() {
      return `https://github.com/ArkEcosystem/ark-explorer/commit/${GIT_VERSION}`
    },
    date() {
      return GIT_DATE
    }
  }
}
</script>
