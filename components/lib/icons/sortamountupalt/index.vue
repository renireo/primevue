<template>
    <svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg" v-bind="pti()">
        <g :clipPath="`url(#${pathId})`">
            <path d="M19,16.25H5a.74.74,0,0,1-.69-.46A.75.75,0,0,1,4.47,15l7-7a.75.75,0,0,1,1.06,0l7,7a.75.75,0,0,1,.16.82A.74.74,0,0,1,19,16.25ZM6.81,14.75H17.19L12,9.56Z"/>
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
    name: 'SortAmountUpAltIcon',
    extends: BaseIcon,
    computed: {
        pathId() {
            return `pv_icon_clip_${UniqueComponentId()}`;
        }
    }
};
</script>
