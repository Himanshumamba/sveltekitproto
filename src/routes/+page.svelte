<script>

  import Header from '$lib/Header.svelte';

</script>

<style global>
.text_bwerben{
    display: inline-block;
    opacity: 0.8;
    max-width: 90%;
    text-align:right;
    margin: 0 auto;
}




  .hero-banner {
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
    background: linear-gradient(102deg, #EBF4FF 0%, #E6FFFA 100%);
    height: 80vh;
    clip-path: polygon(0 0, 100% 0, 100% 80%, 0 100%);
    width: 100%;
  }


  .hero-banner::after {
    content: "";
    position: absolute;
    bottom: -25px;
    left: 0;
    width: 100%;
    height: 40px;
    background: #fff;
  }

  .content {
    text-align: left;
    margin-right: 6rem;
  }

  .three-buttons {
    display: flex;
    justify-content: center;
    margin: 2rem;
    flex-wrap: wrap;
  }

  h1 {
    max-width: 100%;
    font-weight: bold;
    font-size: clamp(28px, 6vw, 48px);
    line-height: clamp(32px, 7vw, 64px);
    letter-spacing: 1.5px;
    padding-bottom: 1rem;
    color: #2D3748;
    font-family: 'Lato', sans-serif;
  }

  button {
    background-color: #fff;
    color: #319795ad;
    border: 1px solid #CBD5E0;
    border-radius: 3px;
    padding: 10px 30px;
    cursor: pointer;
    font-size: clamp(12px, 2vw, 16px);
    transition: background-color 0.3s, color 0.3s;
  }

  button.active {
    background-color: #81E6D9;
    color: white;
  }

  .hero_button {
    background: linear-gradient(95deg, #319795 0%, #3182CE 100%);
    border: none;
    border-radius: 12px;
    font-family: 'Lato', sans-serif;
    font-size: clamp(14px, 2vw, 17px);
    color: #fff;
    padding: 10px 20px;
    width: auto;
    cursor: pointer;
    margin: 1rem 0;
  }

  .hero-image {
 
    width: 30%;
    border-radius: 50%;
  }

  .heading-section {
    text-align: center;
    margin-top: 30px;
    margin-bottom: 4rem;

    padding: 20px;
  }

  .heading-section h2 {
    font-size: clamp(21px, 4vw, 36px);
    font-family: 'Lato', sans-serif;
    letter-spacing: 0px;
    color: #4A5568;
    opacity: 1;
    margin: 0;
  }
.timeline {
    display: flex;
    flex-direction: column;
    align-items: center;
}
.bubble{
display: flex;
    height: 50vh;
    justify-content: center;
    position: relative;
    top: -9rem;
    background: transparent linear-gradient(104deg, #E6FFFA 0%, #EBF4FF 100%) 0% 0% no-repeat padding-box;
clip-path: polygon(49.2% 3.8%, 84.9% 1%, 100.1% 4.8%, 99.6% 81%, 84.6% 96%, 55.7% 95.8%, 0% 100.3%, 0% 0%);    border-radius: 0% 40% 45% 0%;
}
.timeline-item {
    display: flex;
    justify-content: center;
    align-items: center;
    gap:10rem;
    max-width: 1200px;

}
.arrow.last_arrow{
    transform: translate(2rem, -13rem);
}


.numberlist {
  display: inline-flex;
  justify-content: center; 
  align-items:center;
  width: 13vw; 
  height: 13vw; 
  border-radius: 50%;
  background-color: #F7FAFC; /*changed  as  the xd color is nto visible8*/
  color: #718096; 
  font-size: 130px; 
  margin-right: 2vw; 
}
.numberlist_two {
  display: inline-flex;
  justify-content: center; 
  align-items: center;
  color: black; 
  font-size: 130px; 
  color:#718096;
  padding-left:1rem;


}
.text {
    text-align: left;
}

.image {
    flex: 1;
    display: flex;
    justify-content: center;
}

.image img {
    max-width: 100%;
    height: auto;
}

.Erstellen {
    margin-left: -5rem;
    z-index:+1;
}

.Nhead_sub{
color:#718096;
padding-bottom:2rem;
 font-family: 'Lato', sans-serif;



}

@media(min-width:768px){

  .timeline .one{
        align-items: baseline;
  }
  .text_bwerben{
    display: inline-block;
    max-width: 90%;
    margin: 0 auto;
    position: relative;
    left: -5rem;
    top: -2rem;
}
 .timeline-item.one {
    margin-left: -12rem;
}
.timeline-item.second{
  gap:15rem;
}

.arrow {
      display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    height:50vh;
    left: -8rem;
    top: -2rem;
    z-index: +1;

}

.timeline-item.third{
 transform: translate(0rem, -25rem);
 gap:0

}
}

  @media (max-width: 768px) {
    .text_bwerben,.Erstellen,Verwalte {
      font-size:19px
    }

    .Erstellen {
display: inline-block;
    opacity: 0.8;
    margin: 0 auto;
}
.hero-banner {
        margin-top: 4rem;        
        clip-path: none;
    }

    .bubble {
    display: flex;
    height: 64vh;
    justify-content: center;
    margin-bottom:2rem;
    position: unset;
    padding-left: 20px;
    top: -7rem;
    background: transparent linear-gradient(104deg, #E6FFFA 0%, #EBF4FF 100%) 0% 0% no-repeat;
clip-path: polygon(36.4% 6.5%, 69.9% 2.8%, 100.1% 1.8%, 100.1% 89.5%, 84.7% 96.5%, 39.3% 98.4%, 0.4% 93.5%, 0% 0%);
        border-radius: 0;
}

.timeline.sectend{
    padding-left: 1rem;
}
      .content {
        display: flex;
        justify-content: center;
        text-align: center;
        margin: 0 auto;

  }


    .hero_button{
        bottom: -3rem;
      z-index: +1;
    }

  .hero-banner::after {
        position: absolute;

    box-shadow: 0px -3px 6px rgb(177 163 163 / 29%);

  }
       .timeline-item {
        flex-direction: column;
        text-align: center;
        gap:0;
    }

     .text {
    order: 1;
  }

  .timage {
    order: 2;
  }


     .text_sectionone {
    order: 2;
  }

  .timage_sectionone{
    order: 1;
  }



     .image {
        text-align: center;
    }

    .text{
              text-align: center;
        line-height: 1;
        padding-bottom: 2rem;
    }

    .arrow img {
display:none;

    }
    .hero-banner {
      flex-direction: column;
          clip-path: none;

    }

    .hero-image {
          width: 100%;
        margin-top: 20px;
        border-radius: 0;
    }
  .three-buttons {
              margin-top: 6rem;
    }

   
  }

  @media (max-width: 480px) {

    .heading-section{

      margin:0rem;
    }
     .text_bwerben,.Erstellen,Verwalte {
      font-size:15.75px;
    }

    .fixed-container {
      
           position: fixed;
        bottom: 0;
        background-color: #FFFFFF;
        width: 100%;
        left: 50%;
        transform: translateX(-50%);
        z-index: 1000;
}
.numberlist{
 
    font-size: 130px;
    width: max-content;
    background-color:#fff;
}


    .three-buttons {
              margin-top: 6rem;
    }
    .hero-banner {
        clip-path: none;
    }
    .hero-image {
    content: url('/undraw_agreement_aajr@2x.png');
  }
  .profile_one{
      content: url('/undraw_Profile_data_re_v81r@2x.png'); 
      width: 50%;
        margin-bottom: 2rem;


  }
    .profile_two{
      content: url('/undraw_task_31wc@2x.png'); 
      width:70%;
      

  }
      .profile_three{
      content: url('/undraw_personal_file_222m@2x.png'); 
      width:80%;
      

  }
  span.numberlist.one_text {
    align-items: center;
    width:auto;
        background-color: #fff;
        margin-left: -2rem;
    

}

  }
</style>

<!-- Header Section -->
<Header />

<!-- Hero Banner -->
<div class="hero-banner">
  <div class="content">
    <h1>Deine Job <br> website</h1>
    <div class="fixed-container">

    <button class="hero_button">Kostenlos Registrieren</button>
    </div>
  </div>
  
  <img src="/undraw_agreement_aajr.jpg" alt="Hero Image" class="hero-image"  />
</div>

<!-- Pan Buttons -->
<div class="three-buttons">
  <button class="active">Arbeitnehmer</button>
  <button>Arbeitgeber</button>
  <button>Temporärbüro</button>
</div>

<div class="heading-section">
  <h2>Drei einfache Schritte <br>zu deinem neuen Job</h2>
</div>
<section class="timeline one">
    <div class="container">
        <!-- Section 1-->
        <div class="timeline-item one">
            <div class="text_sectionone">

                <p class="Nhead_sub"><span class="numberlist  one_text" >1.</span>
<span class="Erstellen"> Erstellen dein Lebenslauf </span></p>

            </div>
            <div class="timage_sectionone">
                <img src="/profile_first.svg"  alt="Resume Image" class="profile_one">
            </div>
        </div>

        <!-- Arrow connecting section -->
        <div class="arrow">
            <img src="/Gruppe.svg" alt="Arrow">
        </div>

        </section>


        <!-- Section 2-->
        <section class="bubble">
        <div class="timeline-item second">

            <div class="timage">
                <img src="profile_m.svg"  alt="Image" class="profile_two">
            </div>
            <div class="text">
                            <p class="Nhead_sub"><span class="numberlist_two" >2.</span>
<span class="Verwalte">Verwalte deinen Lebenslauf </span></p>

            </div>
        </div>
      </section>
        <!-- Arrow connecting section -->
        <div class="arrow  last_arrow">
            <img src="/Gruppe_2.svg" alt="Arrow">
        </div>

        <!-- Section 3 -->
<section class="timeline  sectend">

     <div class="timeline-item  third">
            <div class="text">

                <p class="Nhead_sub"><span class="numberlist" >3.</span>
                <span class="text_bwerben"> Mit nur einem Klick <br> bewerben <span> </p>
            </div>
            <div class="timage">
                <img src="/profile_last.svg"  alt="Resume Image" class="profile_three">
            </div>
        </div>

    </section>