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
    .outer-container {
        display: flex; /* Enables flexbox */
        justify-content: center; /* Centers content horizontally */
        align-items: center; /* Centers content vertically */
        height: 100vh; /* Full viewport height */
        background-color: #000; /* Optional: Set background color for visibility */
    }

    .container {
        display: block; /* Ensures block layout for left alignment of text */
        max-width: 600px; /* Sets a max width for the container */
        width: 100%; /* Ensures responsiveness */
        text-align: left; /* Aligns text to the left inside the container */
        padding: 20px; /* Optional: Add padding for better spacing */
    }

    .Quotes {
        margin-top: 20px; /* Adds space between quotes and headings */
    }

    h1 {
        font-size: 2rem;
        margin-bottom: 15px;
        color: #ffffff; /* Text color */
    }

    h2 {
        font-size: 1.5rem;
        margin-bottom: 10px;
        color: #ffffff; /* Text color */
    }

    ul {
        list-style-position: inside; /* Ensures bullets align inside */
        padding: 0;
        margin: 0;
        line-height: 1.8;
    }

    li {
        margin-bottom: 10px; 
        font-size: 1rem;
        list-style-type: decimal;
        color: #ffffff; 
    }
</style>
