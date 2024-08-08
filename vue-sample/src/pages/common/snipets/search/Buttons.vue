<template>
    <div class="mt-5 text-center">
        <ClearButton class="me-5" />
        <SearchButton />
    </div>
</template>

<script>
    import ClearButton from '../../parts/buttons/ClearButton';
import SearchButton from '../../parts/buttons/SearchButton';

    export default {
        components: {
            ClearButton,
            SearchButton
        }
    };
</script>
