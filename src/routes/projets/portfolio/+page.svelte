<script>
    import image_logo from "$lib/images/Logo Header.png";
    import image_port from "$lib/images/portfolio.png";
    import image_projets from "$lib/images/Portfolio_projets.png";
    import connexions from "$lib/images/connexions.png";
    let competences = [
        {
            img: "https://upload.wikimedia.org/wikipedia/commons/7/70/Svelte.png",
            nom: "Svelte.JS",
        },
        {
            img: "https://cdn-icons-png.flaticon.com/512/732/732212.png",
            nom: "HTML",
        },
        {
            img: "https://cdn4.iconfinder.com/data/icons/social-media-logos-6/512/121-css3-512.png",
            nom: "CSS",
        },
        {
            img: "https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/JavaScript-logo.png/600px-JavaScript-logo.png",
            nom: "JavaScript",
        },
    ];
</script>

<body
    style="background-image: url({connexions}); background-size:40%; background-repeat:space; background-position:left;"
>
    <main>
        <section id="image_start">
            <h1>Création du portfolio</h1>
        </section>
        <section id="page_projet">
            <div id="projet">
                <h2>Contexte du projet</h2>
                <div class="text">
                    <p>
                        Un projet personnel qui à terme, permettrait de pouvoir
                        <strong
                            >montrer tous mes travaux en développement Web</strong
                        > sur une plateforme qui serait personnalisée et facile d'accès.
                    </p>
                </div>
                <h2>Objectif et Message</h2>
                <div class="text">
                    <p>
                        L'objectif principal de ce projet est bien sûr
                        l'élaboration du portfolio, en <strong
                            >utilisant des outils en full code, principalement
                            Svelte.JS
                        </strong>afin de pouvoir montrer mes compétences en la
                        matière.
                    </p>
                    <p>
                        Le message que je voudrais faire passer dans tout ce
                        portfolio est tout d'abord,<strong
                            >montrer les compétences et le sérieux dont je
                            dispose</strong
                        >, également montrer les talents de développement Web.
                        Et enfin garder le tout dans un
                        <strong>ton moderne et simpliste</strong>.
                    </p>
                </div>
                <div id="Image_et_texte" class="text">
                    <h2>Missions à réaliser</h2>
                    <p>
                        - Mise en place d'une <strong
                            >charte graphique et des logos pour le site</strong
                        >.<br /><br />
                        - Mise en place du projet en
                        <strong>Svelte.JS dans Visual Studio Code</strong>.<br
                        /><br />
                        - Création des différentes pages constituant le portfolio
                        et également le <strong>header et footer</strong>.<br
                        /><br />
                        - Création d'un <strong>formulaire de contact</strong> pour
                        une facilité de communication vers mon adresse mail professionnelle.
                    </p>
                    <img src={image_logo} alt="Logo de charte graphique" />
                    <h3>Logo créé sous Illustrator</h3>
                    <img
                        src={connexions}
                        alt="Motif créé pour la charte graphique"
                    />
                    <h3>Motif graphique de connexions</h3>
                    <img src={image_port} alt="Page d'accueil du Portfolio" />
                    <h3>Page d'accueil du portfolio</h3>
                    <img
                        src={image_projets}
                        alt="Page 'Mes Projets' du portfolio"
                    />
                    <h3>Pages "Mes projets" du portfolio</h3>
                </div>
                <h2>Compétences utilisées :</h2>
                <ul>
                    {#each competences as competence}
                        <li>
                            <img src={competence.img} alt="Compétence" />
                            <h3>{competence.nom}</h3>
                        </li>
                    {/each}
                </ul>
                <h2>Conclusion sur le projet</h2>
                <div id="Image_et_texte" class="text">
                    <p>
                        J'ai beaucoup apprécié travailler sur ce projet, malgré
                        les quelques difficultés lors de la création. Cependant
                        avec <strong
                            >quelques recherches sur plusieurs sources</strong
                        >, j'ai pu trouver des solutions. Ce projet m'a permis
                        d'une part
                        <strong
                            >d'améliorer mes compétences en cette manière de
                            créer des sites Web
                        </strong>mais également d'améliorer ma capacité à
                        <strong>chercher sur différentes sources</strong>.<br
                        /><br />
                        Cependant plusieurs points restent encore à améliorer et
                        également à mettre en place, tels que
                        <strong
                            >la mise en place sur Internet avec un hébergeur
                        </strong>,
                        <strong>retravailler la charte graphique</strong>
                        pour l'étoffer, et également rajouter
                        <strong
                            >un mode sombre pour le site pour améliorer
                            l'accessibilité</strong
                        >.
                    </p>
                </div>
            </div>
        </section>
    </main>
</body>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,400;0,700;0,900;1,400;1,700;1,900&family=Nunito&display=swap");
    body {
        margin: 0em;
        padding: 0em;
        font-family: Montserrat;
        justify-content: center;
    }
    h1 {
        font-size: 3em;
        color: black;
    }
    h2 {
        font-size: 2em;
        text-decoration: underline;
    }
    h3 {
        font-size: 1em;
        text-decoration: underline;
        margin-bottom: 3em;
    }
    p {
        margin-bottom: 2em;
    }

    ul {
        display: flex;
        align-items: center;
        justify-content: center;
        width: 50%;
        flex-wrap: wrap;
        margin-right: 2em;
    }
    li,
    .text {
        width: 50%;
        list-style: none;
        margin-bottom: 3em;
    }

    li img {
        width: 5em;
    }
    #image_start {
        display: flex;
        align-items: center;
        width: 100%;
        flex-wrap: wrap;
        text-align: center;
        padding: 7rem 0 3rem 0;
        flex-direction: column;
        justify-content: center;
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
    }
    #Image_et_texte img {
        width: 100%;
    }
    #Image_et_texte {
        margin-bottom: 3em;
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
    }
</style>
