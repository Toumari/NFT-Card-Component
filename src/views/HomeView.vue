<template>
    <div class="card">
        <div class="img-wrapper">


            <img class="card-img" src="../assets/cube.jpg" alt="">
            <div class="overlay">
                <img src="../assets/eye.png" alt="">
            </div>
        </div>
        <h1 class="card-title">Equilibrium #3429</h1>
        <p class="card-description">Our Equilibrium collection promotes balance and calm.</p>
        <div class="card-price-details">
            <div class="left">
                <img class="small-img" src="../assets/eth-icon2.png" alt="">
                <p class="price">0.041 ETH</p>
            </div>
            <div class="right">
                <img src="../assets/Clock.png" alt="" class="small-img">
                <p class="time-left">3 days left</p>
            </div>


        </div>
        <div class="user-details">
            <img src="../assets/avatar.jpg" alt="" class="avatar">
            <p>Creation of <span>Jack Williams</span></p>
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>
.card {
    max-width: clamp(350px, 90%, 350px);
    box-shadow: 0 0 20px rgba(0, 0, 0, 0.9);
    margin: 0 auto;
    background-color: #15263F;
    padding: 1.5rem;
    border-radius: 15px;
}

.card-img {
    border-radius: 8px;
    width: 100%;
    height: 302px;
    position: relative;
}

.card-img:hover {
    cursor: pointer;
}

.card-title {
    margin-top: 1.5rem;
    font-size: 1.5rem;
    color: white;
    font-weight: 700;
}

.img-wrapper {
    position: relative;
}

.overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 99%;
    background-color: #00FFF8;
    display: flex;
    justify-content: center;
    align-items: center;
    opacity: 0;
    border-radius: 1rem;
    transition: opacity 0.3s;
}

.overlay img {
    width: 75px;
    height: 75px;
    opacity: 1
}

.overlay:hover {
    opacity: 0.6;
}



.card-description {
    margin-top: 1.25rem;
    font-size: 1.1rem;
    line-height: 1.6;
    color: #8BACD9;
}

.card-price-details {
    display: flex;
    justify-content: space-between;
    gap: 0.5rem;
    align-items: center;
    margin-top: 2rem;
    border-bottom: 1px solid #9494a971;
    padding-bottom: 1.5rem;

}

.card-price-details .small-img {
    height: 20px;

}

.price {
    font-size: 1rem;
    color: #00FFF8;
    font-weight: 700;
}

.time-left {
    font-size: 1rem;
    color: #9494a9;

}

.left,
.right {
    gap: 0.5rem;
    display: flex;
    align-items: center;
    justify-content: flex-start;
}

.user-details {
    margin-top: 1.2rem;
    display: flex;
    align-items: center;
    gap: 1rem;
    color: #8BACD9;
}

.user-details span {
    color: white;
    font-weight: 700;
}

.avatar {
    width: 33px;
    height: 33px;
    border-radius: 50%;
    border: 2px solid white;
}
</style>