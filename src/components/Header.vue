<template>
    <header>
    
        <div class="header-container">
            <img class="laravel-img noselect" src="../assets/images/laravel.svg" alt="laravel لاراول">
            <div class="header-title-container noselect" @click="$parent.redirect('https://laravel.4mir.ir')">
                <div class="header-title">
                    راهنمای فارسی لاراول
                </div>
                <div class="header-desc">
                :) اولین راهنمای فارسی لاراول 
                </div>
            </div>
            <title></title>
            
            
            
            <div class="header-object-container"> 
                <a href="https://laravel.com/docs/11.x" target="_blank" class="header-object">مستندات</a>
                <svg @click="toggleDropdown()" class="threedot-menu header-object" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" width="29.957px" height="122.88px" viewBox="0 0 29.957 122.88" enable-background="new 0 0 29.957 122.88" xml:space="preserve"><g><path fill-rule="evenodd" clip-rule="evenodd" d="M14.978,0c8.27,0,14.979,6.708,14.979,14.979c0,8.27-6.709,14.976-14.979,14.976 C6.708,29.954,0,23.249,0,14.979C0,6.708,6.708,0,14.978,0L14.978,0z M14.978,92.926c8.27,0,14.979,6.708,14.979,14.979 s-6.709,14.976-14.979,14.976C6.708,122.88,0,116.175,0,107.904S6.708,92.926,14.978,92.926L14.978,92.926z M14.978,46.463 c8.27,0,14.979,6.708,14.979,14.979s-6.709,14.978-14.979,14.978C6.708,76.419,0,69.712,0,61.441S6.708,46.463,14.978,46.463 L14.978,46.463z"/></g></svg>
                
                <div id="myDropdown" class="dropdown-content">
                    <a target="_blank" href="https://laravel.com/docs/11.x">مستندات</a>
                </div>
            </div>
        </div>
        
    </header>
</template>

<script>

export default {
    name: "Header",
    methods: {
        toggleDropdown() {
            document.getElementById("myDropdown").classList.toggle("show");
        }
    },
}


window.onclick = function(event) {
  if (!event.target.matches(".threedot-menu")) {
    var dropdowns = document.getElementsByClassName("dropdown-content");
    var i;
    for (i = 0; i < dropdowns.length; i++) {
      var openDropdown = dropdowns[i];
      if (openDropdown.classList.contains("show")) {
        openDropdown.classList.remove("show");
      }
    }
  }
};

</script>
