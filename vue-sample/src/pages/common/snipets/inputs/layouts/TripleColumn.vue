<template>
    <b-container class="text-start text-nowrap mb-2">
        <b-row>
            <b-col sm="4">
                <FormGroup
                    :id="id"
                    :value="value"
                    :label="label"
                    label-cols="6"
                    content-cols="6"
                >
                    <slot />
                </FormGroup>
            </b-col>
            <b-col sm="4">
                <FormGroup
                    :id="id"
                    :value="value"
                    :label="label"
                    label-cols="6"
                    content-cols="6"
                >
                    <slot />
                </FormGroup>
            </b-col>
            <b-col sm="4">
                <FormGroup
                    :id="id"
                    :value="value"
                    :label="label"
                    label-cols="6"
                    content-cols="6"
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
