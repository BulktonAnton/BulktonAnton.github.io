  <script>
  import { enhance } from "$app/forms";
  import "elizabot";
  import ElizaBot from "elizabot";
  let eliza = new ElizaBot();
  let chat = [{ user: "eliza", text: eliza.getInitial() }];
  async function write(message) {
        chat.push({user: "me", text: message })
        chat=chat

    // random delay for writing
    await new Promise((r) => setTimeout(r, 1000 + Math.random() * 1000));
        var reply = eliza.transform(message);
        chat.push({ user: "eliza", text: reply });
        
    chat=chat
    

  }
</script>


<svelte:head>
  <link rel="stylesheet" href="/pico.min.css" />
  <style>
    nav {
      margin-left: 10%;
      margin-right: 10%;
    }
    h1 {
  color: #000;
  font-size: min(5vw, 1.2em);
  text-align: center;
  font-style: helvetica;
}
.me {
        font-family: impact;
        background-color: #0000FF;
        font-size: 25px;
        color: #000;
      }
.eliza {
  font-family: serif;
  background-color: #00ccff;
}
  </style>
</svelte:head>

<div class="container">
  <h1>TODO: Complete assignment</h1>
  <div class="scrollable">
    {#each chat as text, i}
    <article class="{chat[i].user}"  >
      <span>
        {chat[i].text}
      </span>
    </article>
    {/each}
  </div>
  <form
    method="post"
    use:enhance={({ form, data, action, cancel }) => {
      /* https://kit.svelte.dev/docs/form-actions#progressive-enhancement */
      cancel(); //don't post anything to server
      const text = data.get("text");
      write(text);
  
      // TODO: reset the form using form.reset()
      form.reset()
    }}
  >
    <input type="text" name="text" />
  </form>
</div>
