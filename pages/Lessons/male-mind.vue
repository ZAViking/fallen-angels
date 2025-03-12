<template>
    <div class="popout-container">
        <div class="popout-content">
            <Nav />

            <h1>Male Mind:</h1>
            <div class="malemind">
                <ul>
                    <li v-for="(malemind, index) in malemind" :key="index">
                        {{ malemind }}
                    </li>
                </ul>
            </div>

            <h1>The Respectful Man:</h1>
            <div class="respectful-man">
                <ul>
                    <li v-for="(respectfulman, index) in respectfulman" :key="index">
                        {{ respectfulman }}
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
            malemind: [
                "Men are not insecure, but territorial.",
            ],
            respectfulman: [
                "Men know how other men are going to be looking at you, or be predators or going to persue you, his right for saying that. Does not mean his insecure. This is a man nature and its ok, and you should have boundaries with yourself knowing that you are exposing yourself.",
                "Most mean wont wife a woman because of the way she presents herself. If you dress provocative, they are going to see you as an object.",
                "Stop calling him insecure, it is their god given right to say 'I dont want my woman to present herself out here because not only is she a representation of me, she is a representation of herself.'",
            ]
        };
    }
};
</script>

<style scoped>
</style>
