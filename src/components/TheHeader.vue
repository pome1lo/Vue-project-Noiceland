<template>
    <header class="header">
        <a href="#">
        <img src="@/assets/LogoHeader.svg"/>
        </a>
        <nav>
        <ul class="navbar">
            <li><a href="#">Home</a></li>
            <li><a href="#">Latest</a></li>
            <li><a href="#">About</a></li>
        </ul>
        </nav>
    </header>
</template>
   
<style scoped lang="scss">
header {
    width: 80%;
    margin: 0% 10%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px;
    nav .navbar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px;
    li {
        margin: 10px 15px;
        :hover {
        transition: .5s;
        color: darkred;
        }
    }
    }  
}
</style>