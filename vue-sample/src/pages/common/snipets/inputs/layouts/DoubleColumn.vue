<template>
    <b-container class="text-start text-nowrap mb-2">
        <b-row>
            <b-col sm="6">
                <FormGroup
                    :id="id"
                    :value="value"
                    :label="label"
                    label-cols="4"
                    content-cols="8"
                >
                    <slot />
                </FormGroup>
            </b-col>
            <b-col sm="6">
                <FormGroup
                    :id="id"
                    :value="value"
                    :label="label"
                    label-cols="4"
                    content-cols="8"
                >
                    <slot />
                </FormGroup>
            </b-col>
        </b-row>
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
