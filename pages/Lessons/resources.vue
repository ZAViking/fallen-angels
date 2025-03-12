<template>
    <div class="popout-container">
        <div class="popout-content">
            <Nav />
            <h1>Resources:</h1>
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
                "Book: The Inner Work of Relationships",
                "Podcast: Mel Robbins Podcast",
                "Podcast: Philosophies for Life",
            ]
        };
    }
};
</script>

<style scoped>
</style>
