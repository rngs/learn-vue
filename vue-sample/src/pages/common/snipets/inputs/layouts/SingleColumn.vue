<template>
    <b-container class="text-nowrap mb-2">
        <FormGroup
            :id="id"
            :value="value"
            :label="label"
            label-cols="2"
            content-cols="5"
        >
            <slot />
        </FormGroup>
    </b-container>
</template>

<script>
    import FormGroup from "../FormGroup";
    export default {
        components: {
            FormGroup
        },
        props: [
            "id",
            "label",
            "value"
        ]
    };
</script>
