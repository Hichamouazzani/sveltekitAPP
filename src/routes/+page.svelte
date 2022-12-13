<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
</script>

<svelte:head>
	<title>Portfolio</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>

<article class="resume" data-page="resume">

       

        <section class="timeline">

          <div class="title-wrapper">
            <div class="icon-box">
              <ion-icon name="book-outline"></ion-icon>
            </div>

            <h3 class="h3">Education</h3>
          </div>

          <ol class="timeline-list">

            <li class="timeline-item">

              <h4 class="h4 timeline-item-title">EIGSI La Rochelle
              </h4>

              <span>2019-2023</span>

              <p class="timeline-text">
                <b>Dominante Entreprise du Futur</b><br>
                - Digitalisation des entreprises<br>
                - Analyse de données<br>
                - Performance industrielle
              </p>

            </li>

            <li class="timeline-item">

              <h4 class="h4 timeline-item-title">CPGE</h4>

              <span>2015-2019</span>

              <p class="timeline-text">
                Classes préparatoires aux grandes écoles 
                filiére (PSI: Physique et Sciences industrielle )
              </p>
            </li>

            <li class="timeline-item">
              <h4 class="h4 timeline-item-title">Baraim errazi (Tétouan,Maroc)</h4>
              <span>2014</span>

              <p class="timeline-text">
                Baccalauréat Sciences mathématiques
              </p>

            </li>

          </ol>

        </section>

        <section class="timeline">

          <div class="title-wrapper">
            <div class="icon-box">
              <ion-icon name="book-outline"></ion-icon>
            </div>

            <h3 class="h3">Projet scolaire</h3>
          </div>

          <ol class="timeline-list">

            <li class="timeline-item">

              <h4 class="h4 timeline-item-title">Projet M.E.S (Manufacturing Excecuting System)</h4>

              

              <p class="timeline-text">
                <b>Tâches réalisées :</b>
                - Evaluer la maturité digitale de l'entreprise<br>
                - Analyser les fonctions nécessaires à implémenter<br>
                - Définir le processus d'implémentation des fonctions analysées
              </p>

            </li>

            <li class="timeline-item">

              <h4 class="h4 timeline-item-title">Projet Data Visualisation avec R Studio</h4>
              
              <p class="timeline-text">
                <b>Tâches réalisées :</b><br>
                - Manipuler les données.<br>
                - Visualiser les données à travers des graphes<br>
              </p>
            </li>

            <li class="timeline-item">

              <h4 class="h4 timeline-item-title">Projet DIGIMAIN</h4>

              

              <p class="timeline-text">
                <b>Tâches réalisées :</b><br>
                - Digitaliser la saisie des informations de la maintenance de l'entreprise PIERRE GUERIN.
                - Transfert des données saisies au base de données de l'entreprise.
              </p>
            </li>

          </ol>

        </section>

        <section class="skill">

          <h3 class="h3 skills-title">My skills</h3>

          <ul class="skills-list content-card">

            <li class="skills-item">

              <div class="title-wrapper">
                <h5 class="h5">Esprit d'analyse</h5>
                
              </div>

              

            </li>

            <li class="skills-item">

              <div class="title-wrapper">
                <h5 class="h5">Data visualisation</h5>
                
              </div>

              

            </li>

            <li class="skills-item">

              <div class="title-wrapper">
                <h5 class="h5">BIG DATA</h5>
                
              </div>
      
            </li>


          </ul>

        </section>

      </article>
	
</section>

<style>

*, *::before, *::after {
  margin: 0;
  padding: 30;
  box-sizing: border-box;
}
:root{

  --text-gradient-yellow: linear-gradient(
    to right, 
    hsl(45, 100%, 72%), 
    hsl(35, 100%, 68%)
  );

  /* solid */

  --jet: hsl(0, 0%, 22%);
  --onyx: hsl(240, 1%, 17%);
  --eerie-black-1: hsl(240, 2%, 13%);
  --eerie-black-2: hsl(240, 2%, 12%);
  --smoky-black: hsl(0, 0%, 7%);
  --white-1: hsl(0, 0%, 100%);
  --white-2: hsl(0, 0%, 98%);
  --orange-yellow-crayola: hsl(45, 100%, 72%);
  --vegas-gold: hsl(45, 54%, 58%);
  --black: hsl(0, 0%, 84%);
  --black: hsla(0, 0%, 84%, 0.7);
  --bittersweet-shimmer: hsl(0, 43%, 51%);

  /**
   * typography
   */

  /* font-family */
  --ff-poppins: 'Poppins', sans-serif;

  /* font-size */
  --fs-1: 18px;
  --fs-2: 18px;
  --fs-3: 18px;
  --fs-4: 18px;
  --fs-5: 18px;
  --fs-6: 18px;
  --fs-7: 18px;
  --fs-8: 18px;

  /* font-weight */
  --fw-300: 300;
  --fw-400: 400;
  --fw-500: 500;
  --fw-600: 600;

}

.article-title { margin-bottom: 30px; }
.timeline { margin-bottom: 30px; }
.timeline .title-wrapper {
  display: flex;
  align-items: center;
  gap: 15px;
  margin-bottom: 25px;
	margin-left:auto;
	margin-right:auto;
}
.timeline-list {
  font-size: var(--fs-6);
  margin-left: auto;
	margin-right:auto;
}
.timeline-item { position: relative; }

.timeline-item:not(:last-child) { margin-bottom: 20px; }

.timeline-item-title {
  font-size: var(--fs-6);
  line-height: 1.3;
  margin-bottom: 7px;
	margin-right: auto; 
	margin-left:auto;
}

.timeline-list span {
  color: var(--vegas-gold);
  font-weight: var(--fw-400);
  line-height: 1.6;
}

.timeline-item:not(:last-child)::before {
  content: "";
  position: absolute;
  top: -25px;
  left: -30px;
  width: 1px;
  height: calc(100% + 50px);
  background: var(--jet);
}

.timeline-item::after {
  content: "";
  position: absolute;
  top: 5px;
  left: -33px;
  height: 6px;
  width: 6px;
  background: var(--text-gradient-yellow);
  border-radius: 50%;
  box-shadow: 0 0 0 4px var(--jet);
}
.timeline-text {
  color: var(--light-gray);
  font-weight: var(--fw-300);
  line-height: 1.6;
}

.skills-title { margin-bottom: 20px; }

.skills-list { padding: 20px; }


.skills-item:not(:last-child) { margin-bottom: 15px; }

.skill .title-wrapper {
  display: flex;
  align-items: center;
  gap: 5px;
  margin-bottom: 8px;
}

.skill .title-wrapper data {
  color: var(--light-gray);
  font-size: var(--fs-7);
  font-weight: var(--fw-300);
}

.skill-progress-bg {
  background: var(--jet);
  width: 100%;
  height: 8px;
  border-radius: 10px;
}

.skill-progress-fill {
  background: var(--text-gradient-yellow);
  height: 100%;
  border-radius: inherit;
}


	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}
  
	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style>
