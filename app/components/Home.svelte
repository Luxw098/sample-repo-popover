<page>
    <actionBar title="Home" />
    <button on:tap={openPopover} >Open Popover</button>
</page>

<script lang="ts">
    import { showPopover } from '@nativescript-community/ui-popover/svelte';
    import Content from './Content.svelte';

    function openPopover() {
        showPopover({
            view: Content,
            props: {}
        });
    };
</script>

<style>

</style>
