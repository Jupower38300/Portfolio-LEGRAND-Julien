<script>
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
    <section
        id="image_start"
        style="background-image: url({connexions}); background-size:40%; background-repeat:no-repeat; background-position:left;"
    >
        <h1>Mes Projets</h1>
    </section>
    <section id="page_projet">
        <div id="projet">
            <div id="text_intro">
                <p>
                    Sur cette page, découvrez toutes mes réalisations, une
                    <strong>collection variée de sites web </strong>réalisés de
                    différentes manières innovantes. Explorez ces réalisations
                    pour savoir comment je travaille et ce dont je suis capable
                    en tant que développeur web !
                </p>
            </div>
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
        </div>
    </section>
</body>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,400;0,700;0,900;1,400;1,700;1,900&family=Nunito&display=swap");
    body {
        margin: 0em;
        padding: 0em;
        font-family: Montserrat;
    }
    h1 {
        font-size: 3em;
    }
    #text_intro {
        width: 40%;
    }
    #image_start {
        display: flex;
        align-items: center;
        width: 100%;
        flex-wrap: wrap;
        padding: 7rem 0 1rem 0;
        flex-direction: column;
        justify-content: center;
    }
    #projet {
        display: flex;
        align-items: center;
        width: 70%;
        flex-wrap: wrap;
        padding: 5rem 0 7rem 0;
        flex-direction: column;
        justify-content: center;
        text-align: center;
    }
    #projet #Cards {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
    }
    #projet .card {
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
    #projet .card img {
        width: 15em;
    }
    #projet p {
        margin-bottom: 0;
        margin-bottom: 4em;
    }
    #projet .card p {
        margin-top: 0;
        margin-bottom: 1em;
    }
    #projet .card h3 {
        font-size: 1.5em;
        margin-bottom: 0;
    }
    #projet .card a {
        margin-left: 50%;
        margin-right: 50%;
        width: 10em;
    }

    #page_projet {
        display: flex;
        align-items: center;
        width: 100%;
        flex-wrap: wrap;
        padding: 5rem 0 7rem 0;
        flex-direction: column;
        justify-content: center;
        text-align: center;
    }
    #projet {
        width: 80%;
        background-color: white;
        display: flex;
        border-radius: 30px;
        flex-direction: column;
        text-align: center;
        align-items: center;
        padding-top: 3em;
        box-shadow: 2em 2em 2em black;
    }
    a,
    a:hover,
    a:checked {
        color: black;
        text-decoration: none;
    }
    .call_to_action {
        margin-right: 2em;
        background-color: #63a9dc;
        color: white;
        padding: 1em;
        border-radius: 2em;
    }
</style>
