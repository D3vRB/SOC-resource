<template>
  <UApp>
    <div class="flex flex-row justify-center items-center fixed px-6 py-6 w-full z-50 bg-green-800">
      <div class="flex justify-end w-7xl px-2 md:px-6">
          <UButton
            color="primary"
            variant="outline"
            to="https://github.com/devrb2202/SOC-resource.git"
            target="_blank"
            icon="i-simple-icons-github"
            aria-label="GitHub"
            :trailing="true"
            size="xl"
          />
      </div>
    </div>
    <UMain class="pt-24">
        <slot />
    </UMain>
  </UApp>

</template>

