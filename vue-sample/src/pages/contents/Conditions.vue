<template>
    <div>
        <Title label="見出し"/>
        <First />
        <Buttons />
    </div>
</template>

<script>
    import Buttons from "../common/snipets/search/Buttons";
import Title from "../common/snipets/titles/Title";
import First from "./conditions/First";

    export default {
        components: {
            Buttons,
            First,
            Title
        }
    };
</script>