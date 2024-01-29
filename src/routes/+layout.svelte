<script>
    import logo_header from "$lib/images/Logo Header.png";
    import logo_footer from "$lib/images/Logo Footer.png";
</script>

<header>
    <a href="/"
        ><img
            id="logo"
            style="width:7em;height:7em;"
            src={logo_header}
            alt="Logo Site"
        /></a
    >
    <nav>
        <ul>
            <li>
                <a href="/about">A propos de moi</a>
            </li>
            <li>
                <a href="/projets">Mes projets</a>
            </li>
            <li>
                <a href="/contact" class="call_to_action">Contact</a>
            </li>
        </ul>
    </nav>
</header>
<slot />

<footer>
    <a href="/"
        ><img
            id="logo_footer"
            style="width:7em;height:7em;"
            src={logo_footer}
            alt="Logo Site"
        /></a
    >
    <nav>
        <ul>
            <li>
                <a href="/about">A propos de moi</a>
            </li>
            <li>
                <a href="/projets">Mes projets</a>
            </li>
            <li>
                <a href="/contact" class="call_to_action">Contact</a>
            </li>
        </ul>
    </nav>
    <hr />
    <p>© Copyright 2023 LEGRAND Julien</p>
</footer>

<style>
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        box-shadow: 0em 1em 4em rgb(68, 68, 68);
        border-radius: 0 0 1em 1em;
        background-color: white;
    }
    footer {
        display: flex;
        justify-content: space-between;
        align-items: center;
        box-shadow: 0em 1em 4em rgb(68, 68, 68);
        border-radius: 1em 1em 0 0;
        flex-direction: column;
        padding-bottom: 1em;
        background-color: white;
    }
    hr {
        width: 15em;
    }
    footer p {
        font-size: 0.9em;
    }

    #logo {
        width: 1 em;
        height: 1 em;
        margin-left: 2em;
    }

    #logo_footer {
        width: 1 em;
        height: 1 em;
        margin-top: 1em;
    }

    ul {
        list-style: none;
        display: flex;
        align-items: center;
        flex-wrap: nowrap;
    }
    li {
        margin-left: 2em;
        display: flex;
        text-align: center;
    }
    a,
    a:hover,
    a:checked {
        color: black;
        text-decoration: none;
        font-weight: bold;
    }
    .call_to_action {
        margin-right: 2em;
        background-color: #63a9dc;
        color: white;
        padding: 1em;
        border-radius: 2em;
    }
</style>
