<script>
  import Card from "./Card.svelte";
  export let loginUser;
</script>

<Card>
  <div class="login__title">
    <h1>Login With Your MetaMask</h1>
  </div>
  <div class="login__para">
    <p>Click the button below to se all your info from your MetaMask Wallet</p>
  </div>
  <div class="login__button">
    <button on:click={loginUser}>Login</button>
  </div>
  <div class="logo">
    <img src="Assetss/logo.png" alt="" />
  </div>
</Card>

<style>
  .login__title h1 {
    padding-bottom: 6px;
  }

  .login__para p {
    padding: 0 40px;
    text-align: center;
  }

  .login__button {
    padding: 20px 0;
  }

  .login__button button {
    background-color: #202142;
    color: white;
    border: none;
    outline: none;
    padding: 10px 30px;
    border-radius: 4px;
    font-weight: 700;
    transition: all 300ms ease;
    border: 2px solid #202142;
    cursor: pointer;
  }

  .login__button button:hover {
    color: #202142;
    background-color: white;
  }

  .logo img {
    width: 100px;
  }
</style>
