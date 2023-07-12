<template>
    <nav>
        <div class="logo">
            <h1>Company</h1>
        </div>
        <ul>
            <li>
                <div class="dropdown">
                    <a href="" class="about">ABOUT</a>
                    <div class="dropdown-content">
                        <a href="#">HISTORY</a>
                        <a href="#">VISION MISSION</a>
                    </div>
                </div>
            </li>
            <li><a href="">OUR WORK</a></li>
            <li><a href="">OUR TEAM</a></li>
            <li><a href="">CONTACT</a></li>
        </ul>
    </nav>
</template>
  
<script>
export default {
    name: 'HeaderVue',

}
</script>
  
  
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap");

/* NAV */

nav {
    display: flex;
    width: 100%;
    justify-content: space-between;
    padding-bottom: 5px;
    padding-top: 20px;
}

nav .logo {
    padding-left: 20vh;
}

nav .logo h1 {
    font-size: 18px;
    font-family: "Roboto", sans-serif;
    font-weight: 500;
}

nav ul {
    padding-right: 14vh;
}

nav ul li {
    list-style-type: none;
    display: inline;
    font-size: 14px;
    font-family: "Roboto", sans-serif;
    font-weight: 400;
    padding-right: 50px;
    text-decoration: none;
}

nav ul li a {
    text-decoration: none;
    color: rgb(63, 63, 63);
}

.about {
    background-color: #fff;
    font-size: 14px;
    border: none;
    color: rgb(63, 63, 63);
    
}

.dropdown {
    position: relative;
    display: inline-block;
    font-size: 14px;
    height: 20px;
}

.dropdown-content {
    display: none;
    position: absolute;
    background-color: #f1f1f1;
    min-width: 160px;
    z-index: 1;
}

.dropdown-content a {
    color: black;
    padding: 12px 16px;
    text-decoration: none;
    display: block;
    font-size: 14px;
}

.dropdown-content a:hover {
    color: #ddd;
    background-color: rgb(63, 63, 63);

}

.dropdown:hover .dropdown-content {
    display: block;
}
</style>
  