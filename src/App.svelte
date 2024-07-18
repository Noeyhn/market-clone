<script>
  import Login from "./pages/login.svelte";
  import Main from "./pages/main.svelte";
  import NotFound from "./pages/NotFound.svelte";
  import Signup from "./pages/signup.svelte";
  import Write from "./pages/write.svelte";
  import Router from "svelte-spa-router";
  import "./css/style.css";

  const routes = {
    "/": Main,
    "/login": Login,
    "/signup": Signup,
    "/write": Write,
    "*": NotFound,
  };
</script>

<Router {routes} />
