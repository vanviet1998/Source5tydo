<template>
  <a-form :form="form">
    <a-input v-model="firstname" placeholder="Họ"/>
    <a-input v-model="lastname" placeholder="Tên"/>
    <a-input v-model="phone" placeholder="Số điện thoại"/>
    <a-input v-model="address" placeholder="Địa chỉ"/>
    <a-form-item>
      <a-date-picker v-model="birthday" placeholder="Ngày sinh"/>
    </a-form-item>
    <a-input v-model="email" placeholder="Email"/>
    <a-input v-model="fb" placeholder="Facebook"/>
    <!-- <a-form-item :wrapper-col="{ span: 12, offset: 5 }">
      <a-button type="primary" v-on:click="handleSubmit">
        Submit
      </a-button>
    </a-form-item>
    {{firstname}} -->
  </a-form>
</template>
<script>
import Topnav from './Topnav'

export default {
  name: 'Store',
  components: {
    Topnav
  },
  methods: {
    handleSubmit (event) {
      console.log('event', event)
    }
  }
}
</script>
<style scoped>
.ant-form {
  padding: 15px;
}
.ant-input {
  border: none;
  border-bottom: 1px solid #d9d9d9;
  border-radius: 0;
  outline: none;
  margin-bottom: 15px;
}
.ant-input:focus {
  box-shadow: none;
}
.ant-calendar-picker {
  width: 100%;
}
.ant-form-item{
  margin: 0;
}
</style>
