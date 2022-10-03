<script>
  import Card from "./Card.svelte";
  import { Balance } from "svelte-web3/components";

  export let selectedAccount;
  export let chainId;
</script>

<Card>
  <div class="info__block">
    <div class="info__title">
      <h4>Adress Name:</h4>
    </div>
    <div class="info__result">
      <p>{$selectedAccount}</p>
    </div>
  </div>
  <div class="info__block">
    <div class="info__title">
      <h4>chainId:</h4>
    </div>
    <div class="info__result">
      <p>{$chainId}</p>
    </div>
  </div>
  <div class="info__block">
    <div class="info__title">
      <h4>Balance:</h4>
    </div>
    <div class="info__result">
      <p><Balance address={$selectedAccount} /></p>
    </div>
  </div>
</Card>

<style>
  .info__block {
    display: flex;
  }

  .info__title h4 {
    padding-right: 10px;
  }
</style>
