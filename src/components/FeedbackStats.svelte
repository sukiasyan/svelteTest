<script>
    export let count
    export let average
</script>

<div class="feedback-stats">
    <h4 >{count} Reviews</h4>
    <h4>Rating Average: {average}</h4>
</div>

<style>
    .feedback-stats {
        display: flex;
        justify-content: space-between;
        align-items: center;
        /* padding: 20px;
        background-color: #fff;
        border-radius: 15px;
        color: #333;
        margin: 20px 0;
        position: relative; */
    }
</style>