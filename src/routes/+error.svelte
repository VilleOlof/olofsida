<script>
    import { page } from '$app/stores';
</script>

<div>
    <h1 id=wrong>Something Went Wrong...</h1>

    <h1>{$page.status}</h1>
    <p>{$page.error?.message}</p>
</div>

<style lang="scss">
    div {
        display: flex;
        justify-content: flex-start;
        align-items: center;
        flex-direction: column;

        margin: 0;
        padding: 0;
        margin-top: 8rem;
    }

    #wrong {
        font-size: 3.5em;
    }

    h1 {
        font-size: 6em;
        margin: 1rem;
        padding: 0;
    }

    p {
        font-size: 2em;
        margin: 1rem;
        padding: 0;
    }

</style>