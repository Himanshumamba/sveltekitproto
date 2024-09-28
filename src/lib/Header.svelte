<script>
  import { onMount } from 'svelte';

let isButtonInHeader = false; 
let scrollDistanceThreshold = 300; 

function handleScroll() {
  if (window.scrollY > scrollDistanceThreshold) {
    isButtonInHeader = true;
  } else {
    isButtonInHeader = false; 
  }
}

onMount(() => {
  window.addEventListener('scroll', handleScroll);

  // Clean up the scroll listener when the component is destroyed
  return () => {
    window.removeEventListener('scroll', handleScroll);
  };
});

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
  padding: 5px 0; 
  z-index: 1000; 

  display: flex;                 
  justify-content: flex-end;      
  align-items: center;  
  height: 70px;                   
  line-height: 70px;            
    
  }

  .hero_button_top {
  margin-right: 10px;
  margin-bottom:0;             
  padding: 10px 15px;            
  background-color: #007bff;    
  color: #fff;                    
  border: none;                
  border-radius: 5px;            
  cursor: pointer;                
}


.login-link {
  text-decoration: none;         
  padding: 10px 15px;             
      color: #319795;
           font-family: 'Lato', sans-serif;


}
@media (min-width: 768px) {

.hero_button_top {
    background: #fff;
    border: 1px solid #CBD5E0;
    border-radius: 12px;
    font-family: 'Lato', sans-serif;
   font-size: clamp(14px, 2vw, 17px);
    color: #319795;
    padding: 10px 20px;
    width: auto;
    cursor: pointer;
     margin: 1rem 0;
}

}


@media (max-width: 768px) {
    header {
    padding: 28px 0;
    z-index: 1000;
    border-bottom-left-radius: 1em;
    border-bottom-right-radius: 1em;
    }
}
</style>

<header>
  <hr class="gradient-hr" />
  {#if isButtonInHeader}
    <button class="hero_button_top">Kostenlos Registrieren</button>
  {/if}
  <a href="#" class="login-link">Login</a>
</header>