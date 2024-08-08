<template>
    <b-form-radio-group
        :id="id"
        :name="name"
        :options="options"
        v-model="computedSelected"
        plain
      />
</template>

<script>
    export default {
        props: [
            "id",
            "name",
            "selected",
            "options"
        ],
        computed: {
            computedSelected: {
                get () {
                    return this.$props.selected
                },
                set (value) {
                    this.$emit("change", value);
                }
            }
        }
    };
</script>
