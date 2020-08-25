<template>
<div>
    <site-header @tab="tab_changed($event)" />
    <member-conditions v-if="tab==0" />
    <member-treatment v-else-if="tab==1" />
    <member-symptoms v-else-if="tab==2" />
    <site-footer />
</div>
</template>

<script>
import site_header from '@/components/website/member-header.vue'
import site_footer from '@/components/website/footer.vue'
import member_conditions from '@/components/member/member-conditions.vue'
import member_treatment from '@/components/member/member-treatment.vue'
import member_symptoms from '@/components/member/member-symptoms.vue'
export default {
    layout: "member",
    components: {
        "site-header": site_header,
        "member-conditions": member_conditions,
        "site-footer": site_footer,
        "member-treatment": member_treatment,
        "member-symptoms": member_symptoms,
    },
    data() {
        return {
            tab: 0
        }
    },
    methods: {
        tab_changed(tab) {
            this.tab = tab
        }
    }
}
</script>

<style>

</style>