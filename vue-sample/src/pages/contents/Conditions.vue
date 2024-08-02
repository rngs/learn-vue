<template>
    <div>
        <Title label="見出し"/>
        <First />
    </div>
</template>

<script>
    import Title from "../common/snipets/titles/Title";
import First from "./conditions/First";

    export default {
        components: {
            First,
            Title
        }
    };
</script>