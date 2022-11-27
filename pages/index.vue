<template>
  <div>
    <div class="hidden lg:fixed lg:inset-y-0 lg:flex lg:w-60 lg:flex-col lg:border-r lg:border-gray-200 lg:bg-[#12151D] lg:pt-5 lg:pb-4">
      <div class="flex flex-shrink-0 items-center px-6 mt-5">
        <img class="h-8 w-auto" src="https://i.imgur.com/zPMigV7.png" alt="Brobot Logo" />
      </div>
      <div class="mt-10 flex h-0 flex-1 flex-col overflow-y-auto">
        <div class="px-5 h-full">
          <div class="grid grid-rows-2 h-full">
            <div>
              <div class="flex items-center hover:bg-[#181A25] mb-4 rounded-md active">
                <HomeIcon class="ml-2 h-6 w-6 text-gray-400" />
                <h3 class="py-2 px-3 text-sm text-gray-300 hover:cursor-pointer">Home</h3>
              </div>
              <div class="flex items-center hover:bg-[#181A25] mb-4 rounded-md">
                <AppsIcon class="ml-2 h-6 w-6 text-gray-400" />
                <h3 class="py-2 px-3 text-sm text-gray-300 hover:cursor-pointer">Meus Apps</h3>
              </div>
              <div class="flex items-center hover:bg-[#181A25] mb-4 rounded-md">
                <CalendarIcon class="ml-2 h-6 w-6 text-gray-400" />
                <h3 class="py-2 px-3 text-sm text-gray-300 hover:cursor-pointer">Calendário</h3>
              </div>
              <div class="flex items-center hover:bg-[#181A25] mb-4 rounded-md">
                <CompaniesIcon class="ml-2 h-6 w-6 text-gray-400" />
                <h3 class="py-2 px-3 text-sm text-gray-300 hover:cursor-pointer">Empresas e Filiais</h3>
              </div>
            </div>
            <div class="grid content-end">
              <div class="flex items-center hover:bg-[#181A25] mb-4 rounded-md">
                <HelpCenterIcon class="ml-2 h-6 w-6 text-gray-400" />
                <h3 class="py-2 px-3 text-sm text-gray-300 hover:cursor-pointer">Help Center</h3>
              </div>
              <div class="flex items-center hover:bg-[#181A25] mb-4 rounded-md">
                <ConfigurationIcon class="ml-2 h-6 w-6 text-gray-400" />
                <h3 class="py-2 px-3 text-sm text-gray-300 hover:cursor-pointer">Configurações</h3>
              </div>
              <div class="flex items-center hover:bg-[#181A25] mb-4 rounded-md">
                <ExitIcon class="ml-2 h-6 w-6 text-gray-400" />
                <h3 class="py-2 px-3 text-sm text-gray-300 hover:cursor-pointer">Sair do sistema</h3>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="flex flex-col lg:pl-60">
      <main class="flex-1">
        <div class="grid grid-rows-3 h-full">
          <div class="pt-10 py-4 sm:flex sm:items-center sm:justify-between sm:px-6 lg:px-8 bg-white">
            <div class="flex-1">
              <h1 class="text-xl font-medium leading-6 text-gray-900 sm:truncate">Dashboard</h1>
            </div>
            <div class="mt-4 flex sm:mt-0 sm:ml-4">
              <button type="button" class="sm:order-0 order-1 ml-3 inline-flex items-center rounded-md border border-gray-300 bg-white px-4 py-2 text-sm font-medium text-gray-700 shadow-sm hover:bg-gray-50 focus:outline-none focus:ring-2 focus:ring-purple-500 focus:ring-offset-2 sm:ml-0">Button</button>
            </div>
          </div>
          <div class="border-b border-gray-200 px-4 py-4">Test 1</div>
          <div class="px-4 py-4 bg-[#fafafa] h-full">
            <div>Test</div>
          </div>

        </div>
      </main>
    </div>

  </div>
</template>

<script>
import HomeIcon from "~/components/Icons/HomeIcon";
import AppsIcon from "~/components/Icons/AppsIcon";
import CalendarIcon from "~/components/Icons/CalendarIcon";
import CompaniesIcon from "~/components/Icons/CompaniesIcon";
import ConfigurationIcon from "~/components/Icons/ConfigurationIcon";
import ExitIcon from "~/components/Icons/ExitIcon";
import HelpCenterIcon from "~/components/Icons/HelpCenterIcon";
export default {
  components: {HelpCenterIcon, ExitIcon, ConfigurationIcon, CompaniesIcon, CalendarIcon, AppsIcon, HomeIcon}
}
</script>

<style scoped>
  .active {
    @apply bg-[#181A25];
  }

  .active > h3 {
    @apply text-[#0492F8] font-medium;
  }
</style>
