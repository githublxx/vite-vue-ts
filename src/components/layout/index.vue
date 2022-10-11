<template>
    <div style="width: 100%;">
        <van-nav-bar title="标题" left-text="返回" left-arrow @click-left="onClickLeft" />

    </div>
</template>

<script setup lang="ts">
import type { NavBarProps } from 'vant';

import { ref } from "vue"
const number1 = ref<number>(1)
console.log(number1);

const aa = ref<boolean>(false);


let tup1: [string, number, boolean]
tup1 = ['小明', 12, false]

let x: any = 'hah'
// x.ifItExit()
// x.toFixed()
// console.log(x.toFixed());

let b: (string | number | boolean)[]
b = ['2121', 2, false,]

let c: void
c = undefined
// c = null

const onClickLeft = (e: MouseEvent): void => {
    console.log(e);

    console.log('onclick');
}
</script>

<style scoped>

</style>