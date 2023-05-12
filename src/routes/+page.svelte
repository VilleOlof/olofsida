<script lang="ts">

</script>

<picture id=BG>
    <source srcset="Home-Background.webp" type="image/webp" />
    <source srcset="Home-Background.jpg" type="image/jpeg" />
    <img id=BG src="Home-Background.jpg" alt="Minecraft Background" />
</picture>

<div id="homeBG">

    <div id="homeContent">
        <div id="title">
            <h1 id=BigHead>Olof</h1> <img src="favicon.png" alt="">
        </div>

        <p>
            Välkommen till min fantastiska hemsida! <br>
            Jag gör Minecraft relaterade videor för alla åldrar!<br>
            Kolla in mina videor <a href="https://youtube.com/@Olof">här!</a>
        </p>
        
        <p>
            Denna hemsidan är fortfarande under utveckling. <br>
            Denna är temporär och kommer att bytas ut mot en ny design / layout. <br>
        </p>

        <div id="socials">
            <a id=socialIcon href="https://youtube.com/@Olof"><img src="youtube.svg" alt="Youtube"></a>
            <a id=socialIcon href="https://twitter.com/OfficialOlof"><img src="twitter.svg" alt="Twitter"></a>
        </div>
    </div>

</div>

<style lang="scss">
    #BG {
        position: fixed;
        top: 0;
        left: 0;

        width: 100%;
        height: 100%;
        z-index: -1;

        object-fit: cover;
    }

    #homeBG {
        position: absolute;
        top: 0;
        left: 10%;

        width: 80%;
        height: calc(100% - 3rem);
        z-index: 1;

        background-color: rgba(0, 0, 0, 0.6);

        transition: 0.2s;
    }

    #homeContent {
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
        align-items: center;

        margin-top: 2rem;
    }

    #BigHead {
        font-size: 5rem;

        margin: 3rem 0 1rem;
    }

    #title {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;

        img {
            margin-top: 1.5rem;

            width: 5rem;
            height: auto;

            margin-left: 1rem;

            filter: drop-shadow(0.5rem 0.5rem 0.5rem rgba(0, 0, 0, 0.5));
        }
    }

    p {
        font-size: 1.5rem;

        width: 80%;
        text-align: center;
    }

    #socials {
        display: flex;
        flex-direction: row;

        img {
            width: 4rem;
            height: auto;

            margin: 0 1rem;

            filter: invert(100%) drop-shadow(0.5rem 0.5rem 0.5rem rgba(0, 0, 0, 0.5));

            transition: filter 0.15s;

            &:hover {
                filter: invert(50%);
            }
        }
    }

    @media screen and (max-width: 400px) {

        #homeBG {
            left: 0;
            width: 100%;
        }

        #BigHead {
            font-size: 3rem;
        }

        p {
            font-size: 1rem;
        }

        #socials {
            flex-direction: column;
        }
    }
</style>
