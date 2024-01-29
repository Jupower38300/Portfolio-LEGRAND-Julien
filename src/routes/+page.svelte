<script>
    import image_pres from "$lib/images/Photo_site.png";
    import image_astral from "$lib/images/Astral_Frontiers.png";
    import image_port from "$lib/images/portfolio.png";
    import image_weplay from "$lib/images/WePlayForCharity.png";
    import connexions from "$lib/images/connexions.png";
    let projets = [
        {
            nom: "Astral Frontiers",
            date: "Avril 2023",
            desc: "Site pour une agence de voyage interstellaire pour la planète GJ1002",
            image: image_astral,
            link: "/projets/astral_frontiers",
        },
        {
            nom: "Portfolio",
            date: "Décembre 2023",
            desc: "Site de démonstration de mon portfolio pour mes réalisations",
            image: image_port,
            link: "/projets/portfolio",
        },
        {
            nom: "WePlayForCharity",
            date: "Avril 2022",
            desc: "Site pour l'association de livestreams caritatives WePlayForCharity",
            image: image_weplay,
            link: "/projets/weplayforcharity",
        },
    ];
</script>

<body>
    <main>
        <section
            id="presentation"
            style="background-image: url({connexions}); background-size:30%; background-repeat:no-repeat; background-position:right;"
        >
            <div
                id="image"
                style="background-image: url({connexions}); background-size:120%; display:flex;"
            >
                <img src={image_pres} alt="LEGRAND Julien" />
            </div>
            <div id="contenu">
                <h1>LEGRAND Julien, Étudiant en Développement Web</h1>
                <p>
                    Bonjour à vous, et bienvenue sur mon portfolio! Je me
                    présente, je suis LEGRAND Julien, actuellement étudiant en
                    seconde année de bachelor Web et Multimédia à
                    MyDigitalSchool Lyon! Ma vocation est le développement web
                </p>
                <a href="/about" class="call_to_action">En savoir plus</a>
            </div>
        </section>
        <hr />
        <section
            id="projets"
            style="background-image: url({connexions}); background-size:50%; background-repeat:no-repeat; background-position:left;"
        >
            <h2>Mes Projets</h2>
            <div id="Cards">
                {#each projets as projet}
                    <div class="card">
                        <img src={projet.image} alt="Projet" />
                        <h3>{projet.nom}</h3>
                        <p><strong>{projet.date}</strong></p>
                        <p>{projet.desc}</p>
                        <a href={projet.link} class="call_to_action"
                            >En savoir plus</a
                        >
                    </div>
                {/each}
            </div>
            <a href="/projets" class="call_to_action">Voir tous les projets</a>
        </section>
        <hr />
        <section id="contact">
            <h2>Si vous appréciez mon travail, pensez à me contacter !</h2>
            <a href="/contact" class="call_to_action">Contactez-moi</a>
        </section>
    </main>
</body>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,400;0,700;0,900;1,400;1,700;1,900&family=Nunito&display=swap");
    body {
        margin: 0em;
        padding: 0em;
        font-family: Montserrat;
    }
    h2 {
        font-size: 2em;
        margin-bottom: 2em;
    }
    h1 {
        font-size: 2.25em;
    }
    a,
    a:hover,
    a:checked {
        color: black;
        text-decoration: none;
    }
    .call_to_action {
        background-color: #63a9dc;
        color: white;
        padding: 1em;
        border-radius: 2em;
        margin-left: 1em;
    }
    #presentation {
        display: flex;
        align-items: center;
        width: 100%;
        flex-wrap: wrap;
        padding: 10rem 0 10rem 0;
        justify-content: space-around;
    }
    #presentation #contenu {
        text-align: center;
        flex-direction: column;
        width: 50%;
    }
    #presentation img {
        width: 20rem;
    }
    #presentation #contenu p {
        margin-top: 2em;
        margin-bottom: 2em;
    }
    #presentation #image {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    hr {
        width: 40%;
        height: 0.5rem;
        color: rgb(24, 24, 24);
        background-color: rgb(45, 45, 45);
        border-radius: 2rem;
    }

    #projets {
        display: flex;
        align-items: center;
        width: 100%;
        flex-wrap: wrap;
        padding: 7rem 0 7rem 0;
        flex-direction: column;
        justify-content: center;
    }
    #projets h2 {
        margin-bottom: 2em;
    }
    #projets #Cards {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
        margin-bottom: 2em;
        margin-left: 2em;
    }
    #projets .card {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        width: 20em;
        height: 25em;
        border-radius: 20px;
        margin-bottom: 20px;
        margin-right: 20px;
        text-align: center;
        background-color: rgb(245, 245, 245);
        box-shadow: 1em 1em 2em rgba(150, 150, 150, 0.481);
    }
    #projets .card img {
        width: 15em;
    }
    #projets .card p {
        margin-top: 0;
    }
    #projets .card h3 {
        font-size: 1.5em;
        margin-bottom: 0;
    }
    #projets .card a {
        margin-left: 50%;
        margin-right: 50%;
        width: 10em;
    }

    #contact {
        display: flex;
        align-items: center;
        width: 100%;
        flex-wrap: wrap;
        padding: 7rem 0 7rem 0;
        flex-direction: column;
        justify-content: center;
        text-align: center;
    }
</style>
