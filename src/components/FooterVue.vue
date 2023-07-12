<template>
    <footer>
        <div class="container">
            <h4>
                Copyright &copy; 2016. PT Company
            </h4>
            <div class="rows">
                <div class="colom">
                    <img src="../assets/facebook-official.png" alt="" srcset="" width="20px">
                </div>
                <div class="colom">
                    <img src="../assets/twitter.png" alt="" srcset="" width="25px">
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "FooterVue"
}
</script>

<style scoped>
    footer{
        margin-top: 10vh;
        height: 100px;
        width: 100%;
        display: flex;    
        background-color: rgb(61, 61, 61);
    }

    h4{
        text-align: center;
        font-size: 13px;
        font-weight: 600;
        color: white;
    }

    .rows{
        justify-content: center;
        display: flex;
        padding-top: 5px;
        width: 100%;
        gap: 15px;
    }

    .container{
        margin-top: auto;
        margin-bottom: auto;
    }
</style>