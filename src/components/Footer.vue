<template>
    <footer>
        <div class=" container">
                <button>sign-up now!</button>

                <nav>
                    <ul class="flex">
                        <h4>follow us</h4>
                        <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="fb"></a></li>
                        <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter"></a></li>
                        <li><a > <img src="../assets/img/footer-youtube.png" alt="youtube"></a></li>
                        <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a></li>
                        <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="locator"></a></li>
                    </ul>
                </nav>
            </div>   
    </footer>
</template>

<script>

export default {
    name: "Footer",
}
</script>

<style scoped lang="scss">

footer {
    padding: 55px;
    background: rgb(46, 43, 43);     
}

/*button*/
 button {
     text-transform: uppercase;
     color: #fff;
     padding: 12px;
     background: transparent;
     border: 3px solid rgb(34, 110, 211);
     position: relative;
     bottom: 5px;
     cursor: pointer;
     transition: .3s;
 }

 button:hover {
     background:rgb(199, 199, 199);
     color:rgb(34, 110, 211);
 }


/*links*/
nav {
    display: flex;
    justify-content: flex-end;
    flex-grow: 1;

}

ul {
    display: flex;
}

h4 {
    text-transform: uppercase;  
    position: relative;
    top: 8px;
    right: 20px;
    color:rgb(34, 110, 211);
}


li {
    margin: 0 10px;
}    

 
img {
    width: 25px;
}


</style>