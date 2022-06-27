
    <!-- Material Icons -->
<link
  rel="stylesheet"
  href="https://fonts.googleapis.com/icon?family=Material+Icons"
/>
<!-- Roboto -->
<link
  rel="stylesheet"
  href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,600,700"
/>
<!-- Roboto Mono -->
<link
  rel="stylesheet"
  href="https://fonts.googleapis.com/css?family=Roboto+Mono"
/>
    <!-- SMUI Styles -->
    <link rel="stylesheet" href="/smui.css" />

<div class="grid items-center content-center min-h-screen">
<Dialog
  bind:open
  aria-labelledby="default-focus-title"
  aria-describedby="default-focus-content"
>
  <Title id="default-focus-title">Advice</Title>
  <Content id="default-focus-content">
    Build something today, even if it sucks.
  </Content>
  <Actions>
    <Button on:click={() => (response = 'I will make you! Do it!')}>
      <Label>You Can't Make Me</Label>
    </Button>
    <Button
      defaultAction
      use={[InitialFocus]}
      on:click={() => (response = 'It will be glorious.')}
    >
      <Label>I Will</Label>
    </Button>
  </Actions>
</Dialog>

<Button on:click={() => (open = true)}>
  <Label>Open Dialog</Label>
</Button>

<pre class="status">Response: {response}</pre>
</div>

<script lang="ts">
  import Dialog, { Title, Content, Actions, InitialFocus } from '@smui/dialog';
  import Button, { Label } from '@smui/button';

  let open = false;
  let response = 'Nothing yet.';
</script>
