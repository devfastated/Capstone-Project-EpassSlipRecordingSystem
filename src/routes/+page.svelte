<script>
   let message = '...';
   let imageVisible = false;
   
    function showMessage(){
        message += "    Iloveyou";

    }

    function toggleImage(){
      let  image = document.getElementById('image'); 
      image.src = '/love.png';
      if (imageVisible){
        image.style.display = 'none';
        imageVisible = false;
      } else {
        image.style.display = 'block';
        imageVisible = true;
      }
    }

</script>



<h1>My name is  {message}  </h1> 

<button on:click={showMessage}>Click me! I have surprise</button>
<img id="image" alt="">
<button on:click={toggleImage}>Show Image</button>

<style>
    h1{
        color: goldenrod;
        font-family: 'Comic Sans MS', cursive;
        font-size: 2em;
    }

    button {
        border: 1px solid black;
        padding: 2px ;
        border-radius: 5px;
        
        
    }
</style>


