<script>


    let count = 0;
    function increment(){
       count++;
       console.log('count', count);
    }
</script>
<div class="ma">

    <button on:click={increment}>Total: {count}</button>


</div>

<style>
    .ma{
        display: fle;
        align-items: center;
        width: 100px;
    }
</style>