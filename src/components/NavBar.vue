<template>
    <v-app-bar app color="black" dark flat class="px-12">
        <v-btn>
            <v-icon color="yellow" left class="mr-2">fas fa-suitcase</v-icon>DEAN
        </v-btn>
        <v-spacer></v-spacer>
        <v-btn text @click="scroll('home')" class="text-yellow">Home</v-btn>
        <v-btn text @click="scroll('about')">About</v-btn>
        <v-btn text @click="scroll('what-i-do')">What I Do</v-btn>
        <v-btn text @click="scroll('contact')">Contact</v-btn>
    </v-app-bar>
</template>

<script>
export default{
    methods: {
        scroll(scrll) {
            const element = document.getElementById(scrll);
            element.scrollIntoView({behavior: "smooth"});
        }
    }
}
</script>

<style>

</style>