<template>
    <div>
        <Example :component="ExSimple" :code="ExSimpleCode"/>

        <ApiView :data="api"/>
        <VariablesView :data="variables"/>
    </div>
</template>


<script>
    import api from './api/navbar'
    import variables from './variables/navbar'

    import ExSimple from './examples/ExSimple'
    import ExSimpleCode from '!!raw-loader!./examples/ExSimple'
    
    export default {
        data() {
            return {
                api,
                variables,
                ExSimple,
                ExSimpleCode
            }
        },
    }
</script>
