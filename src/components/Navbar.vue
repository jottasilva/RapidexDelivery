<template>
    <div id="navbar">
        <nav>
            <section class="logo"/>
            <section class="menu">
                <ul>
                    <li>Promoções</li>
                    <li>Estabelecimentos</li>
                    <li>Seu Delivery</li>
                </ul>
                <section class="search"/>
                <section class="bag">
                    <div><span>12</span></div>
                </section>
            </section>
        </nav>
    </div>
   
</template>
<script></script>
<style scoped>
    #navbar{
        display: flex;
        height: auto;
        justify-content: center;
        align-items: center;
        width: 100%;
        min-height: 200px;
    }
    nav{
        display: flex;
        justify-content: space-between;
        flex-direction: row;
        width: var(--width);
    }
    .logo{
        width: 200px;
        height:70px;
        background:url('../assets/imgs/logo.svg') no-repeat;
        background-size: cover;
        margin: 20px;
    }
    .menu{
        display: flex;
        align-items: center;
        justify-content: center;
        min-width:40%;
    }
    .menu ul{
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        gap: 30px;
        border-radius: 60px;
        padding: 10px;
    }
    .menu ul li{
        display: flex;
        align-items: center;
        flex-direction: row;
        padding:10px;
        justify-content: center;
        font-family: "Roboto", sans-serif;
        font-weight: 600;
        color: var(--azul);
        font-size: 0.9rem;
        letter-spacing: 1px;
        list-style: none;
        cursor: pointer;
        text-transform: uppercase;
    }
    .menu ul li:nth-last-child(1){
        background: var(--roxo);
        color: white;
        padding:10px 20px;
        border-radius: 60px;
    }
    .search{
        width: 28px;
        height: 28px;
        background:url('../assets/icons/search.svg') no-repeat top center;
        background-size: cover;
        margin:0 20px 0 30px;
        transition: all 0.2s linear;
    }
    .search:hover{
        background-position: bottom;
    }
    .bag{
        display: flex;
        align-items: flex-end;
        justify-content: flex-start;
        width: 52px;
        height: 52px;
        background: url('../assets/icons/bag.svg') no-repeat top;
        background-size: contain;
        margin:0 0 0 20px;
    }
    .bag div{
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 100%;
        width: 24px;
        height: 24px;
        background:var(--verde);
        color: white;
    }
    .bag div span{
        font-family: "Roboto", sans-serif;
        font-weight: bold;
        font-size: .7rem;
    }
</style>