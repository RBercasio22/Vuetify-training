<template>
    <div class="center-nav">
        <h1>App</h1>
    </div>
    <div class="sidenav">
       
        <a href="#">
            <v-icon icon="mdi-home"></v-icon> 
            Dummy</a>    
        <v-divider :thickness="1" color="white"></v-divider>
        <a href="#">
            <v-icon icon="mdi-web"></v-icon>
        Dummy</a>
        <v-divider :thickness="1" color="white"></v-divider>
        <a href="#">
            <v-icon icon="mdi-account-multiple-check"></v-icon>
            Dummy</a>
        <v-divider :thickness="1" color="white"></v-divider>
        <a href="#">
            <v-icon icon=" mdi-contacts"></v-icon>
            Dummy</a>
        <v-divider :thickness="1" color="white"></v-divider>

    </div>
   
    <div class="main">
        <Todo />
       
    </div>
</template>



<script setup>



</script>


<style scoped>


.center-nav {
    display: flex;
    flex-direction: row;
    text-align: center;
    height: 70px;
    top: 0;
    left: 0;
    right: 0;
    position: fixed;
    background-color: #111;
    color: white;
    justify-content: center;
    align-items: center;
    z-index: 1;
}

/* The sidebar menu */
.sidenav {
  height: 100%; /* Full-height: remove this if you want "auto" height */
  width: 220px; /* Set the width of the sidebar */
  position: fixed; /* Fixed Sidebar (stay in place on scroll) */
  z-index: 1; /* Stay on top */
  top: 70px; /* Stay at the top */
  left: 0;
  background-color: #111; /* Black */
  overflow-x: hidden; /* Disable horizontal scroll */
  padding-top: 10px;

}
/* The navigation menu links */
.sidenav a {
  padding: 6px 8px 6px 16px;
  text-decoration: none;
  font-size: 25px;
  color: #818181;
  display: block;
}

/* When you mouse over the navigation links, change their color */
.sidenav a:hover {
  color: #f1f1f1;
}

/* Style page content */
.main {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-left: 200px; /* Same as the width of the sidebar */
  padding: 20px;
}

/* On smaller screens, where height is less than 450px, change the style of the sidebar (less padding and a smaller font size) */
@media screen and (max-height: 450px) {
  .sidenav {padding-top: 15px; width: 150px;}
  .sidenav a {font-size: 18px;}
  .main p {font-size: 9px;}
}


</style>