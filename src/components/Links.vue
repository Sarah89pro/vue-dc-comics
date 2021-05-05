<template>
     <footer>
         <div class="container flex">
             <div>
                <ul>
                    <h3> dc comics</h3>
                    <li
                    v-for="(item, index) in dsComics"
                    :key="index">
                    <a href="#"> 
                        {{ item.nome }}</a></li>
                </ul>

                <ul>
                    <h3>shop</h3>
                    <li
                    v-for="(item,index) in shop "
                    :key="index"><a href="#"> 
                        {{item.nome }}</a></li>
                </ul>
             </div>   

             <ul>
                 <h3>dc</h3>
                 <li
                 v-for="(item,index) in dc"
                 :key="index"><a href="#">
                     {{ item.nome }}</a></li>
             </ul>
             
             <ul>
                 <h3>sites</h3>
                 <li
                 v-for= "(item,index) in sites"
                 :key= "index" ><a href="#">
                     {{ item.nome }}</a></li>       
             </ul>
         </div>

         <div class="bkg">
            <img src="../assets/img/dc-logo-bg.png" alt="logo-bg">
         </div>
         
     </footer>
  
</template>

<script>
export default {
    name: "Links",
    data() {
        return {
            dsComics: [
                {nome: "characters"},
                {nome: "comics"},
                {nome: "movies"},
                {nome: "tv"},
                {nome: "games"},
                {nome: "videos"},
                {nome: "news"},
            ],
            shop: [
                {nome: "Shop DC"},
                {nome: "Shop DC Collectibles"},
            ],
            dc: [
                {nome: "terms Of Use"},
                {nome: "Privacy policy (New)"},
                {nome: "Ad Choise"},
                {nome: "Jobs"},
                {nome: "subscriptions"},
                {nome: "Talent Workshops"},
                {nome: "CPSC Certificates"},
                {nome: "Ratings"},
                {nome: "Shop Help"},
                {nome: "Contact Us"},
            ],
            sites: [
                 {nome: "DC"},
                 {nome: "MAD Magazine"},
                 {nome: "DC Kids"},
                 {nome: "DC Universe"},
                 {nome: "DC Power Visa"},
            ],

        }
    }
}
</script>

<style scoped lang="scss">

footer {
    position: relative;
    background-image: url(../assets/img/footer-bg.jpg); 
    
}

.container {
    padding: 60px 0;
}

/*links*/

ul {
    padding: 20px;   
}

h3 {
    margin-bottom: 10px;
    color: #fff;
    text-transform: uppercase;
}

a {
  color: rgb(170, 169, 169);
  text-decoration: none;
  text-transform: capitalize;
  font-size: 12px;
  transition: .3s;
}

a:hover {
    color:#fff;
}

/*Dc Logo*/

.bkg {
    width: 530px;
    height: 430px;
    overflow: hidden;
    position: absolute;
    top: 6px;
    left: 50%;
  
}


</style>