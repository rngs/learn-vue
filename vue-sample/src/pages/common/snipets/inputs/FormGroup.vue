<template>
    <b-form-group
        :id="id"
        :label-cols-sm="labelCols"
        :content-cols-sm="contentCols"
        :label="label"
        :label-for="id"
        class="d-flex"
        style="align-items: center;"
    >
         <slot />
    </b-form-group>
</template>

<script>
    export default {
        props: [
            "id",
            "label",
            "labelCols",
            "contentCols"
        ]
    };
</script>
