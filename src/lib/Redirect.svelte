<script lang="ts">
    export let url: string;
    export let https: boolean = true;

    url = https ? url.substring(12, url.length) : url;
</script>

<div>
    <h1>Redirecting To <b>{url}</b></h1>
</div>

<style lang="scss">
    div {
        display: flex;
        justify-content: center;
        align-items: flex-start;
        height: 100vh;

        margin-top: 5rem;

        h1 {
            font-size: 2rem;
            font-weight: 400;
        }
    }
</style>