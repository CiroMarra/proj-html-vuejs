<script>
export default {
  name: 'AppBattle',
  data() {
    return {
        matches: [
        {
                team1: { country: 'Italy', name: 'Ninja Gaming', image: './src/assets/img/t3.png' },
                team2: { country: 'India', name: 'Witch Gaming', image: './src/assets/img/t4.png' },
                game: 'PUBG Battleground',
                description: 'Nulla porttitor accumsan tincidunt. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Vivamus magna justo.',
                time: '10.45',
                date: '1st November, 2022'
            },
            {
                team1: { country: 'Italy', name: 'King Gaming', image: './src/assets/img/t1.png' },
                team2: { country: 'India', name: 'Astro Gaming', image: './src/assets/img/t2.png' },
                game: "Assasin's Creed",
                description: 'Nulla porttitor accumsan tincidunt. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Vivamus magna justo.',
                time: '9.45',
                date: '1st November, 2022'
            },
            {
                team1: { country: 'Italy', name: 'Dgn Gaming', image: './src/assets/img/t5.png' },
                team2: { country: 'India', name: 'Joker Gaming', image: './src/assets/img/t6.png' },
                game: 'Mortal Combat X',
                description: 'Nulla porttitor accumsan tincidunt. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Vivamus magna justo.',
                time: '8.45',
                date: '1st November, 2022'
            },
            {
                team1: { country: 'Italy', name: 'Shark Gaming', image: './src/assets/img/t7.png' },
                team2: { country: 'India', name: 'Krull Gaming', image: './src/assets/img/t8.png' },
                game: 'League of Legends',
                description: 'Nulla porttitor accumsan tincidunt. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Vivamus magna justo.',
                time: '4.45',
                date: '1st November, 2022'
            }
        ]
            
    }

  },
  methods: {
    activateButton(event) {
        event.preventDefault();
  document.querySelectorAll('.ms-link a').forEach(function(link) {
    link.classList.remove('active');
  });
  event.target.classList.add('active');
    }
}
}
</script>

<template>
    <section class="ms-bg-battle-area">
        <div class="container py-2">
            <div class="card text-center">
                <div class="card-text ms-h6">
                    Trending Battle
                </div>
                <div class="card-body">
                    <h1 class="ms-card-title">Upcoming Match</h1>   
                </div>
                <div class="card-text">
                    <ul class="ms-link d-flex justify-content-center gap-3">
                        <li><a href="#" @click="activateButton">All</a></li>
                        <li><a href="#" @click="activateButton">Pubg</a></li>
                        <li><a href="#" @click="activateButton">LOL</a></li>
                        <li><a href="#" @click="activateButton">AC</a></li>
                        <li><a href="#" @click="activateButton">MCX</a></li>
                    </ul>
                </div>
        </div>
        </div>
        <div class="container py-2" v-for="(match, index) in matches" :key="index">
    <div class="ms-bg-col d-flex align-items-center">
        <div class="row d-flex align-items-center">
            <div class="col">
                <div class="card align-items-center" style="width: 16.5rem;">
                    <div class="box-img te">
                        <img :src="match.team1.image" class="card-img-top" alt="...">
                    </div>
                    <div class="ms-card-body px-2" style="width: 12.5rem;">
                        <p class="ms-h6 ">{{ match.team1.country }}</p>
                        <h5 class="ms-text-bold text-center">{{ match.team1.name }}</h5>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="test-box">VS</div>
            </div>
            <div class="col">
                <div class="card align-items-center" style="width: 16.5rem;">
                    <div class="box-img te">
                        <img :src="match.team2.image" class="card-img-top" alt="...">
                    </div>
                    <div class="ms-card-body px-2" style="width: 12.5rem;">
                        <p class="ms-h6 ">{{ match.team2.country }}</p>
                        <h5 class="ms-text-bold text-center">{{ match.team2.name }}</h5>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card align-items-center" style="width: 16.5rem;">
                    <div class="card-body px-5" style="width: 25.5rem;">
                        <h5 class="text-title">{{ match.game }}</h5>
                        <small class="text-white">{{ match.description }}</small>
                    </div>
                </div>
            </div>
        </div>
        <div class="col px-5">
            <div class="end-box d-flex flex-column align-items-center">
                <div>{{ match.time }}</div>
                <p class="box-text">{{ match.date }}</p>
                <div class="d-flex">
                    <div class="circle"><svg class="svg svg-inline--fa fa-youtube" aria-hidden="true" focusable="false" data-prefix="fab" data-icon="youtube" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" data-fa-i2svg=""><path fill="currentColor" d="M549.7 124.1c-6.281-23.65-24.79-42.28-48.28-48.6C458.8 64 288 64 288 64S117.2 64 74.63 75.49c-23.5 6.322-42 24.95-48.28 48.6-11.41 42.87-11.41 132.3-11.41 132.3s0 89.44 11.41 132.3c6.281 23.65 24.79 41.5 48.28 47.82C117.2 448 288 448 288 448s170.8 0 213.4-11.49c23.5-6.321 42-24.17 48.28-47.82 11.41-42.87 11.41-132.3 11.41-132.3s0-89.44-11.41-132.3zm-317.5 213.5V175.2l142.7 81.21-142.7 81.2z"></path></svg></div>
                    <div class="circle"><svg class="svg svg-inline--fa fa-message" aria-hidden="true" focusable="false" data-prefix="fas" data-icon="message" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" data-fa-i2svg=""><path fill="currentColor" d="M511.1 63.1v287.1c0 35.25-28.75 63.1-64 63.1h-144l-124.9 93.68c-7.875 5.75-19.12 .0497-19.12-9.7v-83.98h-96c-35.25 0-64-28.75-64-63.1V63.1c0-35.25 28.75-63.1 64-63.1h384C483.2 0 511.1 28.75 511.1 63.1z"></path></svg></div>
                </div>
            </div>
        </div>
    </div>
</div>
    </section>
</template>

<style scoped>

.end-box:hover{
    background-color: #05c77c;
    color: #202046;
}


.end-box:hover .circle  {
    background-color: #202046;
    color: white;
}

.end-box:hover .svg {
    color: white;
}

.svg {
    width: 30px;
    height: 30px;
    font-size: 30px;
    color: #202046;
}



.circle {
    width: 50px;
    height: 50px;
    background-color: #00ac4d;
    border-radius: 50%;
    margin-right: 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    color: #202046;
    
}

.box-text {
    font-size: 12px;
}

.end-box {
    background-color: #191935;
    width: 200px;
    height: 200px;
    display: flex;
    justify-content: center; 
    position: relative; 
    color: white;
    font-weight: bolder;
    font-size: 30px;


}
.text-title {
    font-size: 32px;
    font-weight: bold;
}

.test-box {
    background-color: #191935;
    width: 100px;
    height: 100px;
    display: flex;
    justify-content: center; 
    align-items: center;
    position: relative; 
    color: #00ac4d;
    font-weight: bolder;
    font-size: 30px;
}



.ms-text-bold {
    font-weight: bold;
    font-size: 25px;
}

.ms-card-body {
    background-color: #333287;
    border-radius: 0% 0% 7% 7%;
    
}

.ms-bg-col {
    background-color: #202046;
    height: 300px;
    border: solid #00ac4d 1px;
    border-radius: 10px;
}

.ms-bg-col:hover {
    background-color: rgba(34, 32, 86, 1);
    border: none;
}

.box-img {
    background-color: #191935;
    width: 200px;
    height: 200px;
    display: flex;
    justify-content: center; 
    align-items: center;
    position: relative; 
    border-radius: 7% 7% 0% 0%;
}

.card-img-top {
    width: 160px;
    height: 160px;
    position: absolute; 
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%); 
}

.ms-card-title {
    font-size: 44px;
    font-weight: bold;
}

.ms-link {
    list-style: none;
    text-decoration: none;
    font-weight: bold;
}
.ms-link a {
    text-decoration: none;
    color: white;
}

.ms-link a.active {
    color: #00ac4d;
}

.ms-bg-battle-area {
    background-color: #191935;
    height: 95vw;
}

.card {
    background-color: transparent;
    color: white;
    border: none;
}

.ms-h6 {
    color: #00ac4d;
    }
</style>