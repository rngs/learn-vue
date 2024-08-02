<template>
        <b-card
            no-body
            bg-variant="transparent"
            text-variant="dark"
            class="my-4 border-0"
        >
            <b-card-body class="d-flex p-0">
                <b-card-sub-title :sub-title="label" class="m-0 fw-bold" />
            </b-card-body>
            <hr class="m-0 mt-1 border-2"/>
        </b-card>
</template>

<script>
    export default {
        props: ["label"]
    };
</script>
