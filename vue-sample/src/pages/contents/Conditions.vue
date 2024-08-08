<template>
    <div>
        <Title label="見出し" v-b-toggle.condisions />
        <b-collapse id="condisions" visible="true">
            <b-form @submit="onSubmit" @reset="onReset">
                <First />
                <Buttons />
            </b-form>
        </b-collapse>
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