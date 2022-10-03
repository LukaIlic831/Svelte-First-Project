<script>
  import { Link } from "svelte-routing";
</script>

<nav>
  <ul>
    <li>
        <Link to="/"><span> Home </span></Link>
      </li>
    <li>
      <Link to="about"><span> About </span></Link>
    </li>
  </ul>
</nav>

<style>
  nav {
    color: white;
    display: flex;
    width: 100%;
    justify-content: center;
    margin-top: 20px;
  }

  ul {
    list-style-type: none;
    display: flex;
  }

  li {
    color: white;
    margin:0 10px;
  }

  li span {
    color: white;
    text-decoration: none;
    font-size: 24px;
  }
</style>
