<template>
    <div id="bottomRight">
        <div class="bg-color-black">
            <div class="d-flex pt-2 pl-2">
                <div class="d-flex">
                    <span class="fs-xl text mx-2">设备运行统计</span>
                    <div class="decoration2">
                        <dv-decoration-2 :reverse="true" style="width:5px;height:6rem;" />
                    </div>
                </div>
            </div>
            <div>
                <BottomRightChart />
            </div>
        </div>
    </div>
</template>

<script>
import BottomRightChart from "@/components/Watch/subcomponents/bottomRightChart";
export default {
    components: {
        BottomRightChart
    }
};
</script>

<style lang="scss" class>
$box-height: 100%;
$box-width: 100%;

#bottomRight {
    padding: 14px 16px;
    height: $box-height;
    width: $box-width;
    border-radius: 5px;

    .bg-color-black {
        height: $box-height;
        border-radius: 10px;
    }

    .text {
        color: #c3cbde;
    }

    //下滑线动态
    .decoration2 {
        position: absolute;
        left: 0.125rem;
    }
}
</style>