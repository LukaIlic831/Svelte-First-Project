<script>
  import {
    defaultEvmStores,
    selectedAccount,
    chainId,
    connected,
  } from "svelte-web3";
  import InfoWrapper from "../Components/InfoWrapper.svelte";
  import LoginBlock from "../Components/LoginBlock.svelte";
  import Navigation from "../Components/Navigation.svelte";

  export let location
  const loginUser = async () => {
    try {
      await defaultEvmStores.setProvider();
    } catch (error) {
      console.log(error);
    }
  };
</script>

<Navigation/>
<LoginBlock {loginUser} />
{#if $connected}
  <InfoWrapper {selectedAccount} {chainId} />
{/if}
