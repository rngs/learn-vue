<template>
    <b-container class="text-start text-nowrap mb-2">
        <b-row>
            <b-col sm="4" v-for="property in properties" :key="property.id">
                <FormGroup
                    :id="property.id"
                    :label="property.label"
                    label-cols="6"
                    content-cols="6"
                >
                     <slot :name="property.id" />
                </FormGroup>
            </b-col>
        </b-row>
        <!-- <b-row>
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
        </b-row> -->
    </b-container>
</template>

<script>
    import FormGroup from "../FormGroup";
    export default {
        components: {
            FormGroup
        },
        props: [
            "properties"
        ]
    };
</script>
