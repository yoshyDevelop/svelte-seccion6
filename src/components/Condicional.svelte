<script lang="ts">
  let show = true;  // Variable que controla si se muestra o no el contenido
</script>

<main>
    <h1>Condicional</h1>
    <h2>Mostrar u ocultar contenido</h2>
    {#if show}
        <p>Este es el contenido que se muestra</p>
        {:else}
            <p>el contenido esta oculto</p>
    {/if}
    <button on:click={() => show = !show}>
        {show ? 'Ocultar' : 'Mostrar'}
    </button>
</main>

<style>

</style>