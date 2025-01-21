<template>
    <div class="Morning-Tasks">
        <ul>
            <li>1st - Alarm rings, get up</li>
            <li>2nd - Make your bed</li>
            <li>3rd - After brushing your teeth, high five yourself. (Don't say a word)</li>
            <li>4th - Drink a full cup of water</li>
            <li>5th - Get outside and take in morning light</li>
            <li>6th - 10 min walk</li>
            <li>7th - Take 15 mins on a project that matters to you</li>
        </ul>
    </div>
</template>

<style scoped>
    .Morning-Tasks {
        display: flex; /* Enables flexbox for centering */
        justify-content: center; /* Centers content horizontally */
        align-items: center; /* Centers content vertically */
        height: 100vh; /* Makes the div take the full viewport height */
        text-align: left; /* Aligns text to the left */
    }

    ul {
        list-style-position: inside; /* Positions bullet points neatly */
        padding: 0; /* Removes default padding from the list */
        margin: 0; /* Removes default margin */
        line-height: 1.8; /* Adds spacing between lines for readability */
    }

    li {
        margin-bottom: 10px; /* Adds spacing between each list item */
    }
</style>
