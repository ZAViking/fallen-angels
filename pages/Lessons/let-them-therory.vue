<template>
    <div class="Morning-Tasks">
        <ul>
            <li>"Let people do what they need to do"</li>
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
