<!-- creazione singola card -->
<template>
    <section>
        <div class="box">
            <div class="img-box">
            <img :src="comics.thumb" :alt="comics.series">
            </div> 
            <h4> {{ comics.series }}</h4>

        </div>
    </section>

    
</template>

<script>
export default {

     name: "AllCards",

     props: ["comics"],
}
</script>

<style scoped lang="scss">
section {
    width: calc( 100% /6);
}

.box {
    margin: 0 auto; 
    width: 300px;   
}

.img-box {
    height: 150px;
    overflow-y: hidden;    
}


img {
    height: 220px;
    width: 160px;
}


h4 {
    font-size: 14px;
    text-transform: uppercase;
    margin: 20px 0;
    width: 60%;
}


</style>


