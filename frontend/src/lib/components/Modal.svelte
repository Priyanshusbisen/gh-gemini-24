<script lang="ts">
    export let dialog: HTMLDialogElement;
</script>

<dialog bind:this={dialog}>
    <button on:click={() => dialog.close()}>x</button>
    <div class="dialog-content">
        <slot></slot>
    </div>
</dialog>

<style>
    button {
        position: absolute;
        left: 3%;
        top: 5%;
        background-color: inherit;
        border: 2px solid var(--clr-4);
        color: var(--clr-4);
        border-radius: .4rem;
    }
    .dialog-content {
        position: absolute;
        left: 3%;
        top: 17%;
    }
</style>