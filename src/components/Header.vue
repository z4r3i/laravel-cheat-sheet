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
            <path class="telegram-icon-path" fill="#000" d="M297.25 326.75l36.75-173.25c3.25-15.25-5.5-21.25-15.5-17.5l-216 83.25c-14.75 5.75-14.5 14-2.5 17.75l55.25 17.25 128.25-80.75c6-4 11.5-1.75 7 2.25l-103.75 93.75-4 57c5.75 0 8.25-2.5 11.25-5.5l27-26 56 41.25c10.25 5.75 17.5 2.75 20.25-9.5zM448 224c0 123.75-100.25 224-224 224s-224-100.25-224-224 100.25-224 224-224 224 100.25 224 224z"></path>
            </svg>
            
            <div class="header-bar"></div>
            
            <div class="header-object-container"> 
                <a href="https://laravel.com/docs/9.x/" target="_blank" class="header-object">مستندات</a>
                <svg @click="toggleDropdown()" class="threedot-menu header-object" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" width="29.957px" height="122.88px" viewBox="0 0 29.957 122.88" enable-background="new 0 0 29.957 122.88" xml:space="preserve"><g><path fill-rule="evenodd" clip-rule="evenodd" d="M14.978,0c8.27,0,14.979,6.708,14.979,14.979c0,8.27-6.709,14.976-14.979,14.976 C6.708,29.954,0,23.249,0,14.979C0,6.708,6.708,0,14.978,0L14.978,0z M14.978,92.926c8.27,0,14.979,6.708,14.979,14.979 s-6.709,14.976-14.979,14.976C6.708,122.88,0,116.175,0,107.904S6.708,92.926,14.978,92.926L14.978,92.926z M14.978,46.463 c8.27,0,14.979,6.708,14.979,14.979s-6.709,14.978-14.979,14.978C6.708,76.419,0,69.712,0,61.441S6.708,46.463,14.978,46.463 L14.978,46.463z"/></g></svg>
                
                <div id="myDropdown" class="dropdown-content">
                    <a target="_blank" href="https://laravel.com/docs/10.x/">مستندات</a>
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
