<script>
    import image_weplay from "$lib/images/WePlayForCharity.png";
    import image_editions from "$lib/images/WePlayForCharity_streamers.png";
    import image_apropos from "$lib/images/WePlayForCharity_association.png";
    let competences = [
        {
            img: "https://static.vecteezy.com/system/resources/previews/020/975/579/original/wordpress-logo-wordpress-icon-transparent-free-png.png",
            nom: "Wordpress",
        },
        {
            img: "https://elementor.com/marketing/wp-content/uploads/2021/10/Elementor-Logo-Symbol-Red.png",
            nom: "Elementor",
        },
    ];
</script>

<body>
    <main>
        <section id="image_start">
            <h1>WePlayForCharity</h1>
        </section>
        <section id="page_projet">
            <div id="projet">
                <h2>Contexte du projet</h2>
                <div class="text">
                    <p>
                        L'association de livestreams caritatifs WePlayForCharity
                        nous ont demandés de les aider pour se diriger vers une
                    <strong>nouvelle charte graphique</strong> et une <strong>refonte de leur site
                        Web entier</strong>.
                    </p>
                </div>
                <h2>Objectif et Message</h2>
                <div class="text">
                    <p>
                        L'objectif principal de cette <strong>refonte de charte
                        graphique</strong> est de permettre à cette association d'avoir
                        un design <strong>plus moderne et plus affirmé, mais également être
                        plus attractifs</strong> pour permettre des plus grandes
                        donations vers les personnes en besoin.
                    </p>
                    <p>
                        Le message que nous voulions faire passer lors de cette
                        refonte est de <strong>montrer une image moderne et épurée de
                        l'association</strong>, avec également une image positive et sérieuse.
                    </p>
                </div>
                <div id="Image_et_texte" class="text">
                    <h2>Missions à réaliser</h2>
                    <p>
                        - Mise en place d'une <strong>nouvelle charte graphique</strong> en lien avec la pateforme Twitch, où les streams se font.<br><br>
                        - Mise en place également d'un <strong>nouveau logo.</strong><br><br>
                        - Mise en place de cettte charte graphique validé par le client sur un <strong>site créé sous Wordpress.</strong>
                    </p>
                    <img src={image_weplay} alt="Page d'accueil du site" />
                    <h3>Page d'accueil du site</h3>
                    <img src={image_editions} alt="Newsletter" />
                    <h3>Page newsletter</h3>
                    <img src={image_apropos} alt="Page d'achat du site" />
                    <h3>Page à propos de l'association</h3>
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
                        Ce projet m'a été bénéfique sur quelques points:<br><br>
                        Tout d'abord, cela m'a entrainé au <strong>travail en coopération</strong> 
                        avec les différents membres de mon groupe, savoir également 
                        comment nous allions nous <strong>répartir les tâches en fonction des 
                        compétences et expertises de chacun</strong>. De plus ce projet m'a permis <strong>d'approfondir
                         d'avantages mes connaissances sur Elementor et wordpress</strong> en poussant 
                         le projet un peu plus que la base pour avoir <strong>un site qualitatif</strong>.<br><br>
                         Cependant une gestion un peu trop fragile à mis ce projet en difficulté 
                         avec les différnets membres du groupe s'inquiétant de <strong>l'avancement des 
                         tâches</strong> pour rendre les livrables à temps. Cette situation m'a permis de 
                         comprendre <strong>l'intêret d'une communication solide et une bonne gestion du 
                         temps et des délais</strong>.
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
        background: linear-gradient(180deg, rgba(120,106,219,1) 0%, rgba(34,34,34,1) 60%);
        justify-content: center;
    }
    h1 {
        font-size: 3em;
        color: white;
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
