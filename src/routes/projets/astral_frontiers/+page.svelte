<script>
    import image_astral from "$lib/images/Astral_Frontiers.png";
    import image_news from "$lib/images/Newsletter.png";
    import image_achat from "$lib/images/Achat.png";
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
            <h1>Astral Frontiers</h1>
        </section>
        <section id="page_projet">
            <div id="projet">
                <h2>Contexte du projet</h2>
                <div class="text">
                    <p>
                        L'agence de voyage Astral Frontiers a été fondée pour
                        permettre aux personnes fortunées de pouvoir échapper à
                        la planète terre, devenue inhabitable depuis la montée
                        trop rapide et l'utilisation excessive de machines
                        polluantes.
                    </p>
                </div>
                <h2>Objectif et Message</h2>
                <div class="text">
                    <p>
                        L'objectif principal de toute cette opération est de
                        <strong>faire connaître notre agence</strong> et donc d'apporter
                        la solution face au problème mondialen proposant nos services
                        interstellaires.
                    </p>
                    <p>
                        Le message que nous voulions faire véhiculer pour cette
                        agence a donc été d'être <strong
                            >une compagnie de confiance</strong
                        >, avec des prix élevés mais abordable pour partir à
                        bord d'une de nos navettes spécialisées.
                    </p>
                </div>
                <div id="Image_et_texte" class="text">
                    <h2>Missions à réaliser</h2>
                    <p>
                        - Mise en place du site à l'aide du logiciel No-Code
                        <strong>Wordpress et Elementor</strong> en lui donnant
                        un aspect "futuriste", pour cela des
                        <strong>plugins supplémentaires </strong>ont été mis en
                        place.<br /><br />
                        - Mise en place d'une page pour un achat et d'un panier en
                        utilisant <strong>le plugin WooCommerce.</strong><br
                        /><br />
                        - Etablissement d'un formulaire de newsletter en utilisant
                        le service <strong>Mailchimp.</strong>
                    </p>
                    <img src={image_astral} alt="Site Wordpress" />
                    <h3>Site sous Wordpress</h3>
                    <img src={image_news} alt="Newsletter" />
                    <h3>Newsletter du site</h3>
                    <img src={image_achat} alt="Page d'achat du site" />
                    <h3>Page d'achat du site</h3>
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
                        Ce projet m'aura été très bénéfique sur certains points:<br
                        /><br />
                        Tout d'abord, j'ai pu apprendre de nouvelles techniques lors
                        du développement de ce site, lors de mes
                        <strong>différentes recherches</strong>
                        pour la création du site, j'ai pu rencontrer des plugins
                        dont je n'avais jamais entendu parler qui m'ont paru pertinents
                        pour le projet. Après mise en place, nous en avons conclu
                        que ça a bien donné l'effet escompté, le "futuriste".
                        <br /><br />
                        Cependant, ce site à encore quelques axes d'amélioration
                        importants que j'ai relevé et utilisé dans les productions
                        futures, le point majeur étant la rapidité du site, qui n'est
                        vraiement pas fameuse, dût aux différents plugins JavaScript
                        qui y sont installés. C'est pour cela que désormais, lors
                        de la création des différnets sites,
                        <strong
                            >j'apporte une attention particulière à la rapidité
                            du site</strong
                        >, car cela est un point majeur dans l'expérience
                        utilisateur.
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
        background-image: url(https://media.istockphoto.com/id/498478219/fr/photo/%C3%A9toiles-dans-le-ciel-de-nuit.jpg?s=612x612&w=0&k=20&c=0xG-QaSg-eNCFu8aheBUSGsnpZVBkOFHAbkDUixlXUA=);
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
