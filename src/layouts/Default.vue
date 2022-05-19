<template>
  <div>
    <slot />
    <footer class="footer has-background-black">
      <div class="columns">
        <div class="column"></div>
        <div class="column has-text-centered">
            <a class="has-text-white" href="https://chat.boonelinux.com/" target="_blank">
              <span class="icon is-large">
                <g-image alt="Mattermost" src="~/images/mattermost-icon.png" />
              </span>
            </a>
            <br/>
            <br/>
            <span class="icon"><g-image src="~/images/Copyleft.svg"/></span> <span class="has-text-white">Highland Linux Use Group 1804-2020</span>
        </div>
        <div class="column"></div>
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
  font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Roboto,
    "Helvetica Neue", Arial, sans-serif;
  background: black;
  margin: 0px;
  padding: 0px;
}
</style>
