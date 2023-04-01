<script lang="ts">
    import { goto } from '$app/navigation';
    import Redirect from '../../lib/Redirect.svelte';

    const URL: string = 'https://twitter.com/OfficialOlof';

    goto(URL);
</script>

<Redirect url={URL}/>