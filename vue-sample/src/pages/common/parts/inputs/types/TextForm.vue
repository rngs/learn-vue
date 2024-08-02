<template>
    <b-form-input :id="id" :value="value"></b-form-input>
</template>

<script>
    export default {
        props: [
            "id",
            "value"
        ]
    };
</script>
