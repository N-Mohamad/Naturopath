<script>
    import { page } from "$app/stores"
    const navs = [
    {
        title: "Accueil",
        href: "/",
    },
    {
        title: "Naturopath",
        href: "/Naturopath",
    },
    {
        title: "Blog",
        href: "/Blog",
    },
    {
        title: "Contacte",
        href: "/contact",
    },
    ];

    $: routeId = $page.route.id;
    
</script>
<nav>
    <div class="container">
    
        <ul>
            {#each navs as {title, href } }
            <li>
            <a {href} class:active={routeId == href} {title}>{title}</a>
            </li>
            {/each}
        </ul>
    </div>
</nav>

<style>
    nav{
        padding: 0.5em;
        background-color: #9eb486;;
        color: white;
        height: 60px;
        display: flex;
    }

    .container {
        display: flex;
        align-items: center;
    }
    ul {
        display: flex;
        margin: 0;
        margin-left: auto;
        list-style: none;
        font-size: 1em;
    }
    li{
        margin-right: 100px;
        font-size: large;
    }

    a {
        text-decoration: none;
        color: rgba(255, 255, 255, 0.584);
        
    }
    .active {
        color: rgb(250, 247, 247);
    }
</style>

