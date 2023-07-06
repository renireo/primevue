<template>
    <svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg" v-bind="pti()">
        <defs>
            <clipPath :id="`${pathId}`">
                <rect width="14" height="14" fill="white" />
            </clipPath>
        </defs>
    </svg>
</template>

<script>
import BaseIcon from 'primevue/baseicon';
import { UniqueComponentId } from 'primevue/utils';

export default {
    name: 'SortAltIcon',
    extends: BaseIcon,
    computed: {
        pathId() {
            return `pv_icon_clip_${UniqueComponentId()}`;
        }
    }
};
</script>
