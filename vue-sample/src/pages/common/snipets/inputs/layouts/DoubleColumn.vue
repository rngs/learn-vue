<template>
    <b-container class="text-start text-nowrap mb-2">
        <b-row>
            <b-col sm="6" v-for="property in properties" :key="property.id">
                <FormGroup
                    :id="property.id"
                    :label="property.label"
                    label-cols="4"
                    content-cols="8"
                >
                     <slot :name="property.id" />
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
            "properties"
        ]
    };
</script>
