<template>
    <span class="rounded-full whitespace-no-wrap uppercase px-2 py-1 text-xs font-bold"
          :style="{ backgroundColor: backgroundColor(), color: textColor() }"
    >{{ __(field.value) }}</span>
</template>

<script>
    import colors from '../mixins/colors';

    export default {
        props: ['resourceName', 'field'],
        mixins: [colors]
    }
</script>
