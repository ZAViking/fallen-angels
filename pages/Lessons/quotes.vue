<template>
    <div class="outer-container">
        <div class="container">
            <h1>Quotes:</h1>
            <div class="quotes">
                <ul>
                    <li v-for="(quote, index) in quotes" :key="index">
                        {{ quote }}
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            quotes: [
                "No one really pays attention to your mental health until you explode. That is the moment you decide to stand up against the abuse and disrespect, you become the villain.",
                "Loving you felt like destiny, losing you felt like justice for the sins I don't remember committing.",
                "Missing you feels like a punishment with no crime, a sentence with no end. But maybe, just maybe, forgetting you will feel like freedom I never knew I needed.",
                "I found my forever, but fate had other plans, turns out I owed the universe a debt I couldn't ignore."
            ]
        };
    }
};
</script>

<style scoped>
</style>
