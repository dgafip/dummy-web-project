<template>
    <h1>Accueil</h1>
    <div class="divider"></div>
    <article>
        <h2>Actualités</h2>
            <div class="flex justify-center">
                <div class="card lg:card-side bg-base-100 shadow-xl w-full xl:w-5/6">
                    <figure><img class="w-40" :src="actualiteImageUrl" alt="Image actualité"/></figure>
                    <div class="card-body">
                        <h2 class="card-title">Nouveau dui accumsan sit amet!</h2>
                        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
                        <div class="card-actions justify-end">
                            <button class="btn btn-primary">En savoir plus</button>
                        </div>
                    </div>
                </div>
            </div>
    </article>
    <div class="divider"></div>
    <section>
        <div class="flex justify-center">
            <div class="carousel w-full sm:w-5/6 md:w-3/4 lg:w-3/5 xl:w-2/5 2xl:w-1/4">
                <div id="slide1" class="carousel-item relative w-full">
                    <div class="grid w-full">
                        <router-link to="/agenda"><h2 class="flex justify-center link link-hover">Agenda</h2></router-link>
                        <router-link to="/agenda"><img :src="agendaImageUrl" class="w-full" /></router-link>
                        <div class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2">
                            <a href="#slide5" class="btn btn-circle">❮</a> 
                            <a href="#slide2" class="btn btn-circle">❯</a>
                        </div>
                    </div>
                </div> 
                <div id="slide2" class="carousel-item relative w-full">
                    <div class="grid w-full">
                        <router-link to="/inscription"><h2 class="flex justify-center link link-hover">Inscription</h2></router-link>
                        <router-link to="/inscription"><img :src="inscriptionImageUrl" class="w-full" /></router-link>
                        <div class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2">
                            <a href="#slide1" class="btn btn-circle">❮</a> 
                            <a href="#slide3" class="btn btn-circle">❯</a>
                        </div>
                    </div>
                </div> 
                <div id="slide3" class="carousel-item relative w-full">
                    <div class="grid w-full">
                        <router-link to="/contactez-nous"><h2 class="flex justify-center link link-hover">Contactez-nous</h2></router-link>
                        <router-link to="/contactez-nous"><img :src="contactImageUrl" class="w-full" /></router-link>
                        <div class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2">
                            <a href="#slide2" class="btn btn-circle">❮</a> 
                            <a href="#slide4" class="btn btn-circle">❯</a>
                        </div>
                    </div>
                </div> 
                <div id="slide4" class="carousel-item relative w-full">
                    <div class="grid w-full">
                        <router-link to="/boutique"><h2 class="flex justify-center link link-hover">Boutique</h2></router-link>
                        <router-link to="/boutique"><img :src="boutiqueImageUrl" class="w-full" /></router-link>
                        <div class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2">
                            <a href="#slide3" class="btn btn-circle">❮</a> 
                            <a href="#slide5" class="btn btn-circle">❯</a>
                        </div>
                    </div>
                </div>
                <div id="slide5" class="carousel-item relative w-full">
                    <div class="grid w-full">
                        <router-link to="/espace-club/login"><h2 class="flex justify-center link-hover">Espace club</h2></router-link>
                        <router-link to="/espace-club/login"><img :src="espaceClubImageUrl" class="w-full" /></router-link>
                        <div class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2">
                            <a href="#slide4" class="btn btn-circle">❮</a> 
                            <a href="#slide1" class="btn btn-circle">❯</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <div class="divider"></div>
    <section>
        <h2>Les partenaires</h2>
    </section>
</template>

<script setup>
    import agendaImageUrl from '@/assets/images/home-page/agenda_image.jpg'
    import inscriptionImageUrl from '@/assets/images/home-page/inscription_image.jpg'
    import contactImageUrl from '@/assets/images/home-page/contact_image.jpg'
    import boutiqueImageUrl from '@/assets/images/home-page/boutique_image.jpg'
    import espaceClubImageUrl from '@/assets/images/home-page/espace_club_image.jpg'
    import actualiteImageUrl from '@/assets/images/home-page/une_actualite.jpg'
</script>
