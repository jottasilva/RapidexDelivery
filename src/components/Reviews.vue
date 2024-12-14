<template>
    <div class="main">
        <article class="profiles">
            <section></section>
            <section></section>
            <section></section>
        </article>
        <article class="reviews">
            <h2>1,582</h2>
            <span>Avaliações feitas</span>
        </article>
        <article class="rating">  
            <h2>4.3 / 5</h2>
            <section class="rings">
                <span>★</span>
                <span>★</span>
                <span>★</span>
                <span>★</span>
                <span>★</span>
            </section>
        </article>
    </div>
</template>
<script>
</script>
<style scoped>
.main {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 10px;
    width: 300px;
    height: 50px;
    padding: 0 0 0 20px;
    background: rgba(255, 255, 255, 0.15);
    backdrop-filter: blur(13.5px);
    -webkit-backdrop-filter: blur(13.5px); 
    border: 1px solid rgba(255, 255, 255, 0.3);
    border-radius: 50px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); 
    margin-left: 30px;
    transition: all .4s ease-in-out;
}
    .main:hover{
        scale: 1.1;
    }
    .profiles{
        display: flex;
        width: 80px;
        align-items: center;
        margin-left: -10px;
        flex-direction: row;
    }
    .profiles section{
        width: 36px;
        height: 36px;
        border-radius: 100%;
        border:1px #ddd solid;
        -webkit-filter: grayscale(1);
        filter: grayscale(1);
        overflow: hidden;
        transition: all 0.5s linear;
    }
    .profiles section:hover:nth-child(2), 
    .profiles section:hover:nth-child(3){
        -webkit-filter: grayscale(0);
        filter: grayscale(0);
        margin-left: -10px;
    }
    .profiles section:nth-child(2), 
    .profiles section:nth-child(3){
        margin-left: -21px;
    }
    .profiles section:nth-child(1){
        background: url('https://img.freepik.com/free-photo/portrait-man-laughing_23-2148859448.jpg') no-repeat center;
        background-size: cover;
        z-index: 3;
    }
    .profiles section:nth-child(2){
        background: url('https://img.freepik.com/free-photo/young-attractive-teenage-girl-wearing-striped-casual-t-shirt-posing-against-pink-wall-with-charming-smile-looks-happy_176532-10915.jpg') no-repeat center;
        background-size: cover;
        z-index: 2;
    }
    .profiles section:nth-child(3){
        background: url('https://img.freepik.com/free-photo/pensive-old-man-with-glasses-cane_23-2148740052.jpg?t=st=1734129496~exp=1734133096~hmac=187a27c60a870c53d2d9b6bc150eb9e19c00a2f628587af461c474344c46f87d&w=740') no-repeat center;
        background-size: cover;
        z-index: 1;
    }
    .reviews{
        display: flex;
        flex-direction: column;
        text-align: left;
        font-family: "Roboto", sans-serif;
        font-weight: 600;
    }
    .reviews h2{
        font-size: 1.4rem;
        color: var(--darkgray);
    }
    .reviews span{
        font-size: .7rem;
        color: #666;
        font-weight: 400;
    }
    .rating{
        display: flex;
        flex-direction: column;
        text-align: left;
        padding: 0 20px 0 0;
    }
    .rating h2{
        font-size: 1.4rem;
        color: var(--darkgray);
    }
    .rings{
        display: flex;
        color: orange;
        gap:2px;
        margin-top: -5px;
    }
    .rings span:nth-last-child(1){
        color: #666;
    }
</style>