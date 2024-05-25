<script lang="ts">
    import Modal from "$lib/components/Modal.svelte";
    import Form from "$lib/components/Form.svelte";
    let dialog: HTMLDialogElement;
</script>

<Modal bind:dialog={dialog}>
    <Form></Form>
</Modal>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<button on:click={() => dialog.showModal()}>
    show dialog
</button>