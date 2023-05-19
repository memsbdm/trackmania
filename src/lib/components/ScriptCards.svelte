<script lang="ts">
    import ScriptCard from "$lib/components/ScriptCard.svelte";

    export let scriptPage;
    export let scripts;
</script>

<ScriptCard scriptDetails={scripts[scriptPage * 3]} />
<ScriptCard scriptDetails={scripts[scriptPage * 3 + 1]} />
<ScriptCard scriptDetails={scripts[scriptPage * 3 + 2]} />
