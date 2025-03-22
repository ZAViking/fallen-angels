<template>
    <div class="popout-container">
        <div class="popout-content">
            <Nav />
            <h1>Laws in life:</h1>
            <div class="laws">
                <ul>
                    <li v-for="(quote, index) in laws" :key="index">
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
            laws: [
                "Murphy Law: The more you fear something, the more likely it is to happen.",
                "Kidlin Law: If you write a problem down clearly and specifically, you have solved half of it.",
                "Gilbert Law: When you take on a task, finding the best ways to achieve the desired result is always your responsibility.",
                "Wilson Law: If you prioritise knowledge over wealth, you will always be rich.",
                "Falkland Law: If you don't have to make a decision, it is better not to make one.",
            ]
        };
    }
};
</script>

<style scoped>
</style>
