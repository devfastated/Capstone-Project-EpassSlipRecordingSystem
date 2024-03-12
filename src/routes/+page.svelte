<script>

    let count = 0;
    function increment(){
       count++;
       console.log('count', count);
    }
</script>   

<div class="text-">
    <button class="btn btn-primary" on:click={increment}>Total: {count}</button>
  </div>


