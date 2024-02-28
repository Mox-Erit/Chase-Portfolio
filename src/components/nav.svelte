<script>
    import { page } from '$app/stores';

    let path;

    $: path = $page.url.pathname;
</script>

<nav>
    <a aria-current={$page.url.pathname === '/' ? 'page' : undefined} href="/"><i class="material-icons">home</i>Homepage</a>

    <a aria-current={$page.url.pathname === '/portfolio' ? 'page' : undefined} href="/portfolio"><i class="material-icons">grid_view</i>Portfolio</a>

    <a aria-current={$page.url.pathname === '/contact' ? 'page' : undefined} href="/contact"><i class="material-icons">mail</i>Contact</a>
</nav>