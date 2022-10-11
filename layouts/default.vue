<template>
    <div>
        <TheHeader @sidenavToggle="displaySidenav = !displaySidenav"/>
        <TheSidenav 
            :show="displaySidenav"
            @close="displaySidenav = false"
        />
        <nuxt />
    </div>
</template>

<script>
import TheHeader from "@/components/Navigation/TheHeader";
import TheSidenav from "@/components/Navigation/TheSidenav";
import TheSideNavToggle from "@/components/Navigation/TheSideNavToggle";
export default {
    components: {
        TheHeader,
        TheSidenav,
        TheSideNavToggle
    },
    data() {
        return {
            displaySidenav: false,
        }
    },
}
</script>

<style lang="scss">
html {
    font-family: 'Roboto', sans-serif;
}
body {
    margin: 0;
}
</style>