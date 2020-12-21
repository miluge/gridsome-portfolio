<template>
  <div class="mx-auto flex flex-col h-screen justify-between">
    <header class="fixed flex justify-between">
      <strong>
        <g-link to="/">{{ $static.metadata.siteName }}</g-link>
      </strong>
      <ThemeSwitcher/>
      <Navbar/>
    </header>
    <main class="mb-auto mt-auto">
      <slot/>
    </main>
    <footer class="flex justify-between my-8">
      <div>
        Copyright
      </div>
      <div>
        Made
      </div>
      <div>
        Links
      </div>
    </footer>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>
body {
  font-family: -apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
  margin:0;
  padding:0;
  line-height: 1.5;
}


.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
}

.nav__link {
  margin-left: 20px;
}
</style>
<script>
import Navbar from "../components/Navbar";
import ThemeSwitcher from "../components/ThemeSwitcher";
export default {
  components: {ThemeSwitcher, Navbar}
}
</script>