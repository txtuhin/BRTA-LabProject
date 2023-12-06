<template>
  <main>
    <div>
      <div class="bg-white border-b border-black">
        <p class="text-black text-center py-0.3">Login and registration are functional. Feel free to test :)</p>
    </div>

      <nav class="bg-black py-4">
        <div class="container mx-auto flex justify-between items-center">
          <div class="text-2xl font-semibold text-white">BRTA</div>
          <!-- Add your navigation links here -->
          <div v-if="!user" class="space-x-4">
            <NuxtLink to='/' class="hover:text-gray-300 text-white">Home</NuxtLink>
            <NuxtLink to='/register' class="hover:text-gray-300 text-white">Register</NuxtLink>
            <NuxtLink class="bQRHNT" to="/login">
              <span class="fKlELC">
                Login
                <svg viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg" class="taKtSf">
                  <path class="chevron" d="M8 13L13 8L8 3" stroke-width="1.5" stroke-linecap="square"
                    stroke-linejoin="round"></path>
                  <path class="stem" d="M12 8L2 8" stroke-width="1.5"></path>
                </svg>
              </span>
            </NuxtLink>
          </div>
          <div v-if="user" class="space-x-4">
            <h6 class="text-white">{{ user.user_metadata.first_name }} {{ user.user_metadata.last_name }}</h6>
            <button @click="logout" class="ieMfVH" :disabled="loading">
              <span class="fKlELC" :class="{ loading: loading }">
                Log out
              </span>
              <svg viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg" class="jjoFVh"
                :class="{ loading: loading }">
                <g fill="none" stroke-width="1.5" stroke-linecap="round" class="faEWLr"
                  style="stroke: var(--icon-color);">
                  <circle stroke-opacity=".2" cx="8" cy="8" r="6"></circle>
                  <circle cx="8" cy="8" r="6" class="VFMrX"></circle>
                </g>
              </svg>
            </button>
          </div>
        </div>
      </nav>
      <slot />
    </div>
  </main>
</template>
<script setup>
const user = useSupabaseUser()
const client = useSupabaseAuthClient()
const logout = async () => {
  const { error } = await client.auth.signOut()
  if (error) {
    return alert('Something went wrong !')
  }
}
</script>