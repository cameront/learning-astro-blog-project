<script lang="ts">
  export let messages: string[] = [];
  let greeting = "";
  function setGreeting() {
    greeting = messages[Math.floor(Math.random() * messages.length)];
  }
</script>

<div>
  <h3>{greeting}! Thank you for visiting!</h3>
  <button on:click={setGreeting}> New Greeting </button>
</div>
