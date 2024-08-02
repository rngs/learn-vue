<template>
        <b-card
            no-body
            border-variant="light"
            bg-variant="light"
            text-variant="dark"
        >
            <b-card-body class="d-flex">
                <b-card-title :title="label" class="m-0 fw-bold" />
            </b-card-body>
        </b-card>
</template>

<script>
    export default {
        props: ["label"]
    };
</script>
