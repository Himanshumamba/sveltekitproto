<script>
</script>

<style>

    .gradient-hr {
  
      height: 5px;
    width: 100%;
    background: linear-gradient(90deg, #319795 0%, #3182CE 100%);
    border: none;
    margin: 0;
    position: absolute;
    box-shadow: none;
    top: 0;
    left: 0;
    right: 0;
    z-index: 1;
    }

    header {
    position: fixed; 
    top: 0; 
    left: 0;
    width: 100%; 
    background: #FFFFFF; 
    box-shadow: 0px 3px 6px rgba(0, 0, 0, 0.29); 
    padding: 20px 0; 
    z-index: 1000; 
    
  }

  header a {
    text-decoration: none;
    color: #319795;
    font-weight: bold;
    padding-right: 1rem;
     display: flex;
     font-family: 'Lato', sans-serif;
    justify-content: flex-end;
  }

@media (max-width: 768px) {
    header {
        position: static; /* Change to static for smaller screens */
        box-shadow: none; /* Optional: Remove shadow if needed */
    }
}
</style>

<header>
<hr class="gradient-hr" />

  <a href="#">Login</a>
</header>
