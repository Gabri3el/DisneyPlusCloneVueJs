<template>
    <Container>
        <div>
            <img src="../assets/view1.png">
        </div>
        <div>
            <img src="../assets/view2.png">
        </div>
        <div>
            <img src="../assets/view3.png">
        </div>
        <div>
            <img src="../assets/view4.png">
        </div>
        <div>
            <img src="../assets/view5.png">
        </div>
    </Container>
</template>

<script>
    export default {
        
    }
</script>

<style lang="css" scoped>
Container{
    margin-top: 30px;
    display: grid;
    grid-template-columns: repeat(5, minmax(0,1fr));
    padding: 30px 80px 0 80px;
    grid-gap: 25px;
}
div{
    border: 3px solid rgba(249 ,249, 249, 0.1);
    border-radius: 10px;  
    box-shadow: rgb(0 0 0/ 69%) 0px 26px 30px -10px,rgb(0 0 0 /73%) 0px 16px 10px -10px; 
    cursor: pointer;
}
img{
    padding: 30px 30px 0 30px;
}

div:hover{
    transform: scale(1.05);
    border-color: rgba(249, 249, 249, 0.8)
}

</style>