<template>
    <div class="component_container menu">
        <div class="wrapper_menu">
            <div class="wrapper_menu_profil p10 mb10">
                <a href="#">
                    <div class="menu_profil_img">
                        <img :src="img_user" alt="">
                    </div>
                    <div class="menu_profil_button">
                        <div class="menu_profil_button_text">
                            <p>Логин</p>
                            <p>000001</p>
                        </div>
                        <div class="menu_profil_button_icon">
                            <span class="arrow arrow_right"></span>
                        </div>
                    </div>
                </a>
            </div>
        </div>
    </div>
</template>

<script>

    import BarBottom from '../BarBottom.vue'

    export default {
        components: {
            BarBottom
        },
        data() {
            return {
                barbottmmenu:{
                    menu:true,
                    map:false,
                    active:'menu'
                },
                img_user:'/images/user.png'
            }
        },
        mounted() {
            console.log('Component mounted.')
        },
        created(){

        },
        methods:{
            
        },
         computed:{
          
        }
    }
</script>

<style>
.component_container.menu {
  max-width: 770px;
  margin: 0 auto;
   min-height: 92vh;
  background-color: #f4f1f19c;
}
   .wrapper_menu_profil a {
    display: flex;
    width: 100%;
    }
    .menu_profil_img {
  flex-basis: 20%;
}
.menu_profil_img img {
  max-width: 40px;
}
.menu_profil_button {
  flex-basis: 80%;
  display: flex;
  justify-content: center;
}
.menu_profil_button_text {
flex: 2;
display: flex;
align-items: center;
flex-direction: column;
}
.menu_profil_button_icon {
  margin-right: 20px;
}
</style>
