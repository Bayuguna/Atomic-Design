<template>
    <div>
        <b-container id="mobile-container">
            <b-row align-v="center">
            <div class="col-2">
               <ButtonIcon :icon="icon" v-b-toggle.sidebar-menu/>
               <Sidebar id="sidebar-menu" :title="title"/>
            </div>
            <div class="col-2">
                <Images id="logo-image" :src="logo" />
            </div>
            <div class="col-8">
                <SearchBar />
            </div>
        </b-row>
        </b-container>
    </div>
</template>

<script>
import Images from "@/components/atoms/Images.vue";
import SearchBar from "@/components/molecules/SearchBars.vue";
import Sidebar from "@/components/molecules/Sidebars.vue";
import ButtonIcon from "@/components/atoms/buttons/ButtonIcon.vue";
export default {
    name: "NavbarMobile",
    components:{
        Images,
        SearchBar,
        Sidebar,
        ButtonIcon
    },
    data:() =>{
        return {
            icon: ['fas', 'bars'],
            title: 'Menu',
            logo: 'umkm_logo.png'
        }
    },
}
</script>

<style scoped>
    #logo-image{
        width: 4rem;
    }
    #mobile-container{
        padding: 0.5rem;
    }
</style>