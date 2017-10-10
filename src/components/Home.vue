<template>
    <div id="home">
        <headers></headers>
        <div class="meau">
            <meau></meau>
        </div>
    </div>
</template>
<script>

import headers from './header/Header'
import meau from './meau/Meau'
export default {
    components: {
        headers,meau
    }
}
</script>

<style lang="scss" scoped>
    .meau{
        width: 200px;
       height: 100%;
    }
    #home{
        width: 100%;
        height: 100%;
    }
</style>
