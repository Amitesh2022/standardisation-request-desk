<script setup lang="ts">
import { onMounted } from 'vue'
import { storeToRefs } from 'pinia'
import { RouterLink, RouterView } from 'vue-router'
import { useDeliveryStore } from './store'
const store = useDeliveryStore()
const { approvedShare, offers, urgent } = storeToRefs(store)
onMounted(store.load)
</script>

<template><div class="shell"><aside><div class="brand">StandardsEuropeEU<span>STANDARDS PIPELINE</span></div><nav><RouterLink to="/">Standardisation requests</RouterLink><RouterLink to="/insights">Standards guidance</RouterLink></nav><div class="health"><i /> Java standardisation request service connected</div></aside><main><header><div><span class="eyebrow">Coordinate policy priorities, technical evidence and stakeholder consensus</span><h1>Standardisation Request Desk</h1></div><button @click="store.addOffer">Add standardisation request</button></header><section class="summary"><article><small>Requests consensus-ready</small><strong>{{ approvedShare }}%</strong><div class="bar"><span :style="{ width: `${approvedShare}%` }" /></div></article><article><small>Requests tracked</small><strong>{{ offers.length }}</strong><p>Shared standards view</p></article><article><small>Evidence gaps</small><strong>{{ urgent }}</strong><p>Needs attention</p></article></section><RouterView /></main></div></template>
