<template>
    <v-container grid-list-lg>
        <v-layout column>
            <v-flex class="text-xs-center display-1 my-5">Pricing</v-flex>
            <v-flex class="text-xs-center display-1 font-weight-black">Plans that scale with your user growth</v-flex>
        </v-layout>
        <v-layout row wrap>
            <v-flex>
                <v-card>
                    <v-img :src="images.rocket1" height="300px">
                        <v-container fluid>
                            <v-layout>
                                <v-flex flexbox>
                                    <span class="subheading purple white--text px-1 py-1">DEVELOPER</span>
                                </v-flex>
                                <v-btn small>Try it</v-btn>
                            </v-layout>
                        </v-container>
                    </v-img>

                    <v-card-title primary-title>
                        <div>
                            <h3 class="headline">Developer</h3>
                            <ul>
                                <li>Includes 1,000 sessions / mo</li>
                                <li>14 day data retention</li>
                            </ul>
                        </div>
                    </v-card-title>
                </v-card>
            </v-flex>

            <v-flex>
                <v-card>
                    <v-img :src="images.rocket2" height="300px">
                        <v-container fluid>
                            <v-layout fill-height>
                                <v-flex flexbox>
                                    <span class="subheading purple white--text px-1 py-1">TEAM</span>
                                </v-flex>
                                <v-btn small>Try it</v-btn>
                            </v-layout>
                        </v-container>
                    </v-img>
                    <v-card-title primary-title>
                        <div>
                            <h3 class="headline">Team</h3>
                            <ul>
                                <li>Starting at 10,000 sessions / mo</li>
                                <li>Starting at 1 month retention</li>
                            </ul>
                        </div>
                    </v-card-title>
                </v-card>
            </v-flex>

            <v-flex>
                <v-card>
                    <v-img :src="images.rocket3" height="300px">
                        <v-container fluid>
                            <v-layout fill-height>
                                <v-flex flexbox>
                                    <span class="subheading purple white--text px-1 py-1">PROFESSIONAL</span>
                                </v-flex>
                                <v-btn small>Try it</v-btn>
                            </v-layout>
                        </v-container>
                    </v-img>
                    <v-card-title primary-title>
                        <div>
                            <h3 class="headline">Professional</h3>
                            <ul>
                                <li>Any volume of Sessions</li>
                                <li>Custom data retention</li>
                                <li>On-premise available</li>
                            </ul>
                        </div>
                    </v-card-title>
                </v-card>
            </v-flex>
        </v-layout>
    </v-container>
</template>

<script>
export default {
    name: 'RocketPlans',
     data() {
        return {
            images: {
                rocket1: require('../assets/rocket_1.jpg'),
                rocket2: require('../assets/rocket_2.jpg'),
                rocket3: require('../assets/rocket_3.jpg')
            }
        }
    }
};
</script>

<style scoped>
</style>