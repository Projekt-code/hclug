<template>
  <div>
    <slot />
    <footer class="footer has-background-black">
      <div class="columns">
        <div class="column"></div>
        <div class="column has-text-centered">
            <a class="has-text-white" href="https://hilug.slack.com/" target="_blank">
              <span class="icon is-large">
                <g-image alt="Slack" src="~/images/slack.png" />
              </span>
            </a>
            &nbsp;
            <a class="has-text-white" href="https://www.meetup.com/High-Country-Linux-Users-Group-HiLUG/" target="_blank">
              <span class="icon is-large">
                <g-image alt="Meetup" src="~/images/meetup.png" />
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
