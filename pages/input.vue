<template>
    <view class="container">
        <uni-s-input label="名字" placeholder="请输入姓名" id="name" @inputValue="getInputValue"></uni-s-input>
        <uni-s-input label="性别" placeholder="请输入性别" id="sex" @inputValue="getInputValue"></uni-s-input>
        <uni-s-input label="年龄" placeholder="请输入年龄" id="age" @inputValue="getInputValue"></uni-s-input>
    </view>
</template>

<script>
import UniSInput from '../components/s-input/uni-s-input.vue'
export default {
    components: {
        UniSInput
    },
    data () {
        return {
            formData: {
                name: '',
                sex: '',
                age: ''
            }
        }
    },
    methods: {
        getInputValue (e) {  // 根据指定id获取相应input的值
            console.log(e)
        }
    }
}
</script>

<style lang="scss" scoped>
</style>
