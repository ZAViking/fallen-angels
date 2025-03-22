<template>
    <div class="popout-container">
        <div class="popout-content">
            <Nav />
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
                "The hardest thing you do, is let go of what you thought would never end. If they choose to go then let them go. Don't beg them to stay. Forcing someone else to stay only deepens the pain when they already gone. Sometimes healing is realizing what wasn't yours to keep. Let go not because you are weak, but because you know you worth more.",
                "No one really pays attention to your mental health until you explode. That is the moment you decide to stand up against the abuse and disrespect, you become the villain.",
                "Loving you felt like destiny, losing you felt like justice for the sins I don't remember committing.",
                "Missing you feels like a punishment with no crime, a sentence with no end. But maybe, just maybe, forgetting you will feel like freedom I never knew I needed.",
                "I found my forever, but fate had other plans, turns out I owed the universe a debt I couldn't ignore.",
                "If you hold onto the past, you stay in the past",
                "You never trutly move on, you never truely get over the hurtful relationships, dont make that stop you from loving someone new",
                "IF you can dream with a damaged mind and love with a broken heart, you deserve this world and all of its treasures",
            ]
        };
    }
};
</script>

<style scoped>
</style>
