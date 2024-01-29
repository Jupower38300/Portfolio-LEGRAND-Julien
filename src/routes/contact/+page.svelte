<script>
    import connexions from "$lib/images/connexions.png";
</script>

<body>
    <main>
        <section
            id="image_start"
            style="background-image: url({connexions}); background-size:50%; background-repeat:no-repeat; background-position:left;"
        >
            <h1>Contact</h1>
        </section>
        <section id="page_projet">
            <div id="projet">
                <div class="text_intro">
                    <h2>
                        Vous appréciez mon travail, si c'est le cas,
                        contactez-moi, ce serait un plaisir de travailler avec
                        vous et de créer des sites ensemble!
                    </h2>
                </div>
                <div class="text">
                    <img
                        src="https://static.vecteezy.com/system/resources/previews/019/923/734/original/telephone-and-mobile-phone-icon-calling-icon-transparent-background-free-png.png"
                        alt="Téléphone"
                    />
                    <h3>0689545285</h3>
                </div>
                <div class="text">
                    <img
                        src="https://www.pngmart.com/files/15/Vector-Email-Symbol-Background-PNG.png"
                        alt="Email"
                    />
                    <h3>julien.legrand@my-digital-school.org</h3>
                </div>
                <div class="text">
                    <img
                        src="https://static.vecteezy.com/system/resources/thumbnails/023/986/900/small/linkedin-logo-linkedin-logo-transparent-linkedin-icon-transparent-free-free-png.png"
                        alt="LinkedIn"
                    />
                    <a href="https://www.linkedin.com/in/julien-legrand2/"
                        ><h3>Mon LinkedIn</h3></a
                    >
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
        padding-top: 3em;
        box-shadow: 2em 2em 2em black;
        justify-content: center;
        align-items: center;
    }
    #page_projet {
        display: flex;
        align-items: center;
        width: 100%;
        flex-wrap: wrap;
        padding: 5rem 0 7rem 0;
        flex-direction: column;
        justify-content: center;
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
    .text {
        width: 100%;
        list-style: none;
        margin-bottom: 3em;
        display: flex;
        justify-content: center;
    }
    .text_intro {
        width: 75%;
        margin-bottom: 3em;
        display: flex;
        justify-content: center;
        text-align: center;
    }
    .text_intro h2 {
        text-decoration: underline;
    }
    .text img {
        width: 4em;
        height: 4em;
    }
    .text h3 {
        margin-left: 2em;
        align-items: center;
    }
    .text a,
    a:hover,
    a:checked {
        color: black;
        text-decoration: none;
    }
</style>
