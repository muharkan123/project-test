<template>
    <div class="container">
        <article>
            <h2>
                OUR VALUES
            </h2>
            <div class="row">
                <div class="col">
                    <div class="card" style="background-color:rgb(206, 89, 89)">
                        <img src="../assets/lightbulb-o.png" alt="" srcset="" width="25px">
                        <h1>INNOVATIVE</h1>
                        <p>
                            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Inventore
                            atque impedit quo aliquam fuga reiciendis!
                        </p>
                    </div>
                </div>
                <div class="col">
                    <div class="card" style="background-color:rgb(105, 201, 105)">
                        <img src="../assets/bank.png" alt="" srcset="" width="45px">
                        <h1>LOYALTY</h1>
                        <p>
                            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Inventore
                            atque impedit quo aliquam fuga reiciendis!
                        </p>
                    </div>
                </div>
                <div class="col">
                    <div class="card" style="background-color:rgb(123, 123, 211)">
                        <img src="../assets/balance-scale.png" alt="" width="50px">
                        <h1>RESPECT</h1>
                        <p>
                            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Inventore
                            atque impedit quo aliquam fuga reiciendis!
                        </p>
                    </div>
                </div>
            </div>
        </article>
    </div>
</template>

<script>
export default {
    name: 'ArticleVue'
}
</script>

<style scoped>
h2 {
    text-align: center;
    margin-top: 90px;
    margin-bottom: 40px;
    font-size: 26px;
    font-weight: bold;
}

.card img {
    display: block;
    margin-left: auto;
    margin-right: auto;
    padding-top: 40px;
    padding-bottom: 10px;
}

.card h1{
    margin-top: 5px;
    text-align: center;
    font-size: 18px;
    font-weight: bold;
    color: white;
}

.card p{
    text-align: center;
    padding: 20px 30px 20px 30px;
    color: white;
    font-weight: 400;
    font-size: 16px;
}
</style>