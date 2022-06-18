<script>
import {
    onMount,
    onDestroy
} from 'svelte'
import {
    FeedbackStore
} from '../stores';
import {
    fade,
    scale
} from 'svelte/transition';
import FeedbackItem from './FeedbackItem.svelte';
// let feedback = [];

// FeedbackStore.subscribe((data) => {
//   feedback = data;
// });

// onDestroy((f) => {
//   unsubscribe();
// });
</script>

{#each $FeedbackStore as fb (fb.id)}
<div in:scale out:fade>
    <FeedbackItem item={fb} on:delete-feedback/>
        </div>
        {/each}
