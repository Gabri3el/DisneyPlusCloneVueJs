<template>
    <Nav>
        <img src="../assets/logo.png">
        <NavMenu>
            <a>
                <b-icon
                    icon="home"
                    size="is-small">
                </b-icon>
                <span>Home</span>
            </a>
             <a>
                <b-icon
                    icon="magnify"
                    size="is-small">
                </b-icon>
                <span>Search</span>
            </a>
             <a>
                <b-icon
                    icon="plus"
                    size="is-small">
                </b-icon>
                <span>My list</span>
            </a>    
            <a>
                <b-icon
                    icon="star"
                    size="is-small">
                </b-icon>
                <span>Originals </span>
            </a>    
            <a>
                <b-icon
                    icon="filmstrip"
                    size="is-small">
                </b-icon>
                <span>Movies </span>
            </a>  
            <a>
                <b-icon
                    icon="television"
                    size="is-small">
                </b-icon>
                <span>Series </span>
            </a> 
        </NavMenu>
        <UserImg>
            <img src="../assets/avatar.png">
        </UserImg>
    </Nav>
</template>

<script>
    export default {
        
    }
</script>

<style lang="css" scoped>
Nav{
    height: 70px;
    background-color: #161924;
    display:flex;
    align-items: center;
    padding: 0 30px;
}
Nav img{
    width:80px
}

navmenu{
    flex: 1;
    margin-left: 25px;
}

navmenu a {
    color: #fff;
    padding: 0 20px;
}

NavMenu span{
    font-family: Avenir-Heavy, sans-serif;
    font-size: 15px;
    letter-spacing: 1.42px
}
NavMenu span:hover{
   border-bottom: 1px solid #fff;
   transition: all 250ms cubic-bezier(0.25, 0.46, 0.45,0.94) 0s;
}

.icon.is-small{
    padding: 0 20px;
    border: none
}

UserImg{
    width: 48px;
    height: 47px;
    cursor: pointer;
}

</style>