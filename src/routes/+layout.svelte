<nav class="layout">
  Access Physical Therapy
  <a prefetch href="/">Home</a>
</nav>

<main>
  <slot />
</main>

<footer class="layout">
  &copy Access Physical Therapy {new Date().getFullYear()}
</footer>

<style>
  :root {
    --muted-green: #61892f;
    --bright-green: #86c232;
    --main-bg-color: #222629;
    --dark-gray: #474b4f;
    --light-gray: #6b6e70;
  }

  nav {
    background: rgba(0, 0, 0, 0.4);
    color: var(--muted-green);
    padding-top: 1rem;
    padding-bottom: 1rem;
  }

  nav > a {
    color: var(--bright-green);
  }

  nav,
  footer {
    text-transform: uppercase;
    font-size: 0.7rem;
    letter-spacing: 0.1px;
    font-weight: 500;
  }

  :global(html) {
    background: var(--main-bg-color);
    overflow-y: scroll;
  }

  :global(article) {
    background-color: var(--dark-gray);
  }

  :global(article > h2) {
    color: var(--bright-green);
  }

  :global(.layout) {
    --width: 700px;
    padding-left: max(1rem, calc(calc(100vw - var(--width)) / 2));
    padding-right: max(1rem, calc(calc(100vw - var(--width)) / 2));
  }

  main {
    margin-bottom: 5rem;
    margin-top: 5vw;
  }

  footer {
    text-align: center;
    margin: 3rem 0;
    color: var(--muted-green);
  }
</style>
