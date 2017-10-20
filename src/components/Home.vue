<template>
    <div id="home">
        <headers></headers>
        <div class="content-wrap">
            <div class="meau-wrap">
                <meau :name="menu"></meau>
            </div>
            <div class="detail-wrap">
                <router-view></router-view>
            </div>
        </div>
    </div>
</template>
<script>

import headers from './header/Header'
import meau from './meau/Meau'
export default {
    data (){
        return{
            menu:'menus'
        }
        
    },
    components: {
        headers,meau
    }
}
</script>

<style lang="scss" scoped>
    .content-wrap{
        width: 100%;
        height: 100%;
        overflow: hidden;
        display: table;
        >div{
            display: table-cell;
            &.meau-wrap{
                width: 250px;
            }
            &.detail-wrap{
                padding: 20px;
            }
        }
    }
    #home{
        width: 100%;
        height: 100%;
    }
</style>
