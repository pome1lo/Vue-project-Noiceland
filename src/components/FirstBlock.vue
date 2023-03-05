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
        justify-content: center;
        grid-template-columns: auto auto;
        width: 100%;
        column-gap: 50px;
        margin-bottom: 50px;
        img {
            width: 721px;
            height: 474px;
            object-fit: cover;
        }
        h1, h2, p {
            text-align: left;
            margin: 25px 0;
        }
        p {
            font-family: 'Source Serif Pro';
            font-style: normal;
            font-weight: 400;
            font-size: 16px;
            line-height: 24px;
            color: #666666;
        }
        h1 {
            font-size: 50px;
            color: black;
            font-family: 'Tenor Sans';
            font-style: normal;
            font-weight: 400;
        }
        h3 {
            text-transform: uppercase;
            color: #999999;
            text-align: left;
            font-size: 15px;
        }
        h2 {
            font-family: 'Libre Franklin';
            font-style: normal;
            font-weight: 700;
            font-size: 15px;
            line-height: 12px;
            letter-spacing: 1px;
            text-transform: uppercase;
            color: #000000;
        }
    }    
</style>