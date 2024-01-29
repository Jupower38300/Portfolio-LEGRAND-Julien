<script>
    import connexions from "$lib/images/connexions.png";
</script>

<body>
    <main>
        <section
            id="image_start"
            style="background-image: url({connexions}); background-size:50%; background-repeat:no-repeat; background-position:left;"
        >
            <h1>A propos de moi</h1>
        </section>
        <section id="page_projet">
            <div id="projet">
                <h2>
                    "Le développement web n'est pas seulement une compétence
                    technique, c'est une forme d'art digital où chaque ligne de
                    code compose la symphonie d'une expérience utilisateur
                    exceptionnelle." - Jeffrey Veen
                </h2>
                <h3>Introduction</h3>
                <div class="text">
                    <p>
                        Bien le bonjour! Je m'appelle Julien Legrand, j'ai
                        19ans, actuellement <strong
                            >étudiant en cycle Web et Multimédia à
                            MyDigitalSchool</strong
                        >
                        et j'ai une vocation dans le développement web. Avec mes
                        deux années dans le cursus, je suis déterminé à apprendre
                        et à m'apénouir dans ce domaine que je trouve passionant.
                        J'ai une maîtrise dnas langages tels que
                        <strong>l'HTML, le CSS, le JavaScript</strong>
                        et des outils no-code tels que
                        <strong
                            >Wordpress avec Elementor ou bien Oxygen Builder</strong
                        >.
                    </p>
                </div>
                <h3>Philosophie</h3>
                <div class="text">
                    <p>
                        Ma philosophie en développement se base sur une
                        <strong
                            >recherche de solutions aux problèmes qui pourraient
                            survenir</strong
                        >
                        et un
                        <strong
                            >apprentissage constant de nouvelles techniques, de
                            langages de programmation</strong
                        > et de la curiosité constante.
                    </p>
                </div>
                <h3>Projet mémorable</h3>
                <div class="text">
                    <p id="text_fin">
                        Parmi tous les projets que j'ai pu réaliser, je suis
                        particulièrement fier du projet de <strong
                            >création de ce portfolio</strong
                        >. Ce projet a été un véritable moyen pour moi d'en
                        apprendre plus sur le développement pur code en
                        utilisant <strong>le framework Svelte.JS</strong>.
                        J'espère qu'il montre le travail qui a été fourni pour
                        sa réalisation, et la qualité que j'aimerai montrer.
                    </p>
                </div>
            </div>
        </section>
    </main>
</body>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,400;0,700;0,900;1,400;1,700;1,900&family=Nunito&display=swap");
    h1 {
        font-size: 3em;
    }
    h2 {
        font-size: 1.4em;
        text-decoration: underline;
        width: 75%;
    }
    h3 {
        font-size: 1.3em;
        text-decoration: underline;
        width: 75%;
    }
    body {
        margin: 0em;
        padding: 0em;
        font-family: Montserrat;
        justify-content: center;
        align-items: center;
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
    #page_projet {
        display: flex;
        align-items: center;
        width: 100%;
        flex-wrap: wrap;
        padding: 5rem 0 7rem 0;
        flex-direction: column;
        justify-content: center;
        text-align: center;
        margin-bottom: 3em;
    }
    #image_start {
        display: flex;
        align-items: center;
        width: 100%;
        flex-wrap: wrap;
        padding: 7rem 0 2rem 0;
        flex-direction: column;
        justify-content: center;
    }
    .text {
        width: 50%;
        list-style: none;
        margin-bottom: 3em;
    }
    #text_fin {
        margin-bottom: 3em;
    }
</style>
