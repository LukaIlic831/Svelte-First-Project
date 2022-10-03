<script>
  import InfoBlock from "./InfoBlock.svelte";
  import { scale } from "svelte/transition";

  export let selectedAccount;
  export let chainId;
</script>

<div class="info__wrapper">
  <div transition:scale>
    <InfoBlock {selectedAccount} {chainId} />
  </div>
</div>

<style>
  .info__wrapper {
    margin-top: 20px;
    display: flex;
    flex-direction: column;
  }
</style>
