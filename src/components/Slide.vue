<template>
    
<article>
        <Reputation />
        <div class="btn-delivery">
            <span>PEDIR AGORA</span>
        </div>
    </article>
</template>
<script>
import Reputation from "./Reviews.vue";
export default{
    components:{
    Reputation
    }
}
</script>
<style scoped>
    article{
        display: flex;
        margin:20px 0;
        align-items: flex-end;
        min-width: var(--width);
        min-height: 520px;
        padding-bottom:30px;
        background: url('../assets/imgs/slide.svg') no-repeat center;
        background-size:cover;  
    }
    .btn-delivery{
        display: flex;
        align-items: center;
        justify-content: center;
        font-family: "Roboto";
        font-size: 1.1rem;
        cursor: pointer;
        color: white;
        padding-right: 30px;
        font-weight: bold;
        letter-spacing:2px;
        width: 200px;
        height: 50px;
        box-shadow: 0 6px 6px rgba(0, 0, 0, 0.1);
        margin-left: 30px;
        border-radius: 50px;
        background:url('../assets/icons/hand-icon.svg') no-repeat center right var(--roxo);
        background-size: 15%;
        background-position-x: 90%;
        transition: all .4s ease-in-out;
    }
    .btn-delivery:hover{
        scale: 1.1;
    }
</style>