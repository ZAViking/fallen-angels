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
                "1. Hard Work - Don't believe in luck, believe in hard work. Stop trying to rush the process or searching for a shortcut. There is none.",
                "2. Patience - If you are losing the patience, you are losing the battle. Patience is the key to success. Firt nothing happens, then it happens slowly and suddenly all at once. Most people give up at stage one.",
                "3. Sacrifice - If you don't sacrifice for what you want, then what you want becomes the sacrifice. The question is: Are you ready to pay it for the life you desire?.",
                "4. Consistency - Consistency is what transforms average into excellence. Without consistency, you will never achieve greatness.",
                "5. Discipline - Motivation gets you going, but discipline keeps you growing. There will be days when you don't feel like it, but you have to do it anyway. You have to push through those days regardless of how you feel.",
                "6. Self Confidence - Confidence is, I'll be fine if they don't like me. There will always be someone judging you for who you are and what you want from life.",
            ]
        };
    }
};
</script>

<style scoped>
</style>
