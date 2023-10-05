<script lang="ts">
    import { goto } from '$app/navigation';
    import Redirect from '../../lib/Redirect.svelte';

    const URL: string = 'https://www.youtube.com/@Olof?sub_confirmation=1';

    goto(URL);
</script>

<Redirect url={URL}/>