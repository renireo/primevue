<template>
    <svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg" v-bind="pti()">
        <g :clipPath="`url(#${pathId})`">
            <path d="M12,16.25a.74.74,0,0,1-.53-.22l-7-7A.75.75,0,0,1,5,7.75H19A.75.75,0,0,1,19.53,9l-7,7A.74.74,0,0,1,12,16.25Zm-5.19-7L12,14.44l5.19-5.19Z"/>
        </g>
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
    name: 'SortAmountDownIcon',
    extends: BaseIcon,
    computed: {
        pathId() {
            return `pv_icon_clip_${UniqueComponentId()}`;
        }
    }
};
</script>
