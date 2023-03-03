<template>
    <div class="first-block">
        <img src="@/assets/FirstBlock.png"/>
        <div>
            <h3>Illustration</h3>
            <h1>Japan House opens in mountainside to foster peak creativity.</h1>
            <p>Enim omittam qui id, ex quo atqui dictas complectitur. Nec ad timeam accusata, hinc justo falli id eum, ferri novum molestie eos cu.</p>
            <h2>BY Reta Torphy</h2>
        </div>
    </div>
</template>
   
<style scoped lang="scss">
    .first-block {
        display: grid;
        width: 80%;
        column-gap: 30px;
        margin: 50px 11.5%;
        grid-template-columns: 55% 45%;
        img {
            width: 100%;
        }
        h1, h2, p {
            text-align: left;
            margin: 25px 0;
        }
        h1 {
            font-size: 50px;
                    }
        h3 {
            text-transform: uppercase;
            color: #999999;
            text-align: left;
        }
        h2 {
            text-transform: uppercase;
        }
    }    
</style>