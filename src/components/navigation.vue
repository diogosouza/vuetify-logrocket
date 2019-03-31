<template>
    <span>
        <v-navigation-drawer app v-model="drawer">
            <v-list>
                <template v-for="(menu, i) in menus">
                    <v-list-tile :key="i">
                        <v-list-tile-content>
                            {{menu.value}}
                        </v-list-tile-content>
                    </v-list-tile>
                    <v-divider :key="`divider-${i}`"></v-divider>
                </template>
            </v-list>
        </v-navigation-drawer>
        <v-toolbar app dark>
            <v-toolbar-side-icon class="hidden-md-and-up" @click="drawer = !drawer"></v-toolbar-side-icon>
            <v-spacer class="hidden-md-and-up"></v-spacer>
            <v-img src="https://assets.logrocket.io/img/logo.png" max-width="120px" max-height="25px"></v-img>
            <v-btn flat class="hidden-sm-and-down">Pricing</v-btn>
            <v-spacer class="hidden-sm-and-down"></v-spacer>
            <v-btn flat class="hidden-sm-and-down">Customers</v-btn>
            <v-btn flat class="hidden-sm-and-down">Docs</v-btn>
            <v-btn flat class="hidden-sm-and-down">Blog</v-btn>
            <v-btn flat class="hidden-sm-and-down">Login</v-btn>
            <v-btn color="purple darken-3" class="hidden-sm-and-down">Sign Up</v-btn>
        </v-toolbar>
    </span>
</template>

<script>
export default {
    name: 'RocketNavigation',
    data() {
        return {
            drawer: false,
            menus: [
                { value: 'Pricing' },
                { value: 'Customers' },
                { value: 'Docs' },
                { value: 'Blog' },
                { value: 'Login' },
                { value: 'Sign Up' }
            ]
        };
    }
};
</script>

<style scoped>
</style>