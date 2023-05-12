<script lang="ts">
    import '../app.scss';
</script>

<slot></slot>

<footer>
    <p>© 2023 Olof - <a href="mailto:kontaktolofspelar@gmail.com">kontaktolofspelar@gmail.com</a></p>
</footer>

<style lang="scss">
    footer {
        z-index: 5;

        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;

        position: fixed;
        bottom: 0;
        left: 0;
        right: 0;

        background-color: #222;
        height: 3rem;

        box-shadow: 0 0 0.5rem 0.5rem rgba(3, 3, 3, 0.534);
    }

    p {
        &:first-child {
            margin-right: 2rem;
        }

        &:last-child {
            margin-left: 2rem;
        }

        color: #fff;

        white-space: nowrap;
    }

    @media screen and (max-width: 400px) {
        p {
            &:last-child {
                display: none;
            }
        }
    }
</style>

