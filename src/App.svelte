<script lang="ts">
  let data = ''
</script>

<div>
  <textarea
    bind:value={data}
    cols={80}
    rows={8}
  />
  <br />
  {#if data}
    <img src={`data:;base64,${data}`} />
  {/if}
</div>
