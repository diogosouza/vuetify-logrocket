<template>
    <v-app>
        <rocket-navigation></rocket-navigation>
        <rocket-plans></rocket-plans>
        <rocket-footer></rocket-footer>
    </v-app>
</template>

<script>
import RocketNavigation from '@/components/navigation';
import RocketPlans from '@/components/plans';
import RocketFooter from '@/components/footer';

export default {
    name: 'LogRocketApp',
    components: {
        RocketNavigation,
        RocketPlans,
        RocketFooter
    }
};
</script>

<style>
</style>