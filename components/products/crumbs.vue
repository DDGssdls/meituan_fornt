<template>
  <div class="m-crumbs">
    <el-breadcrumb separator=">">
      <el-breadcrumb-item :to="{ path: '/' }">{{ city.replace('市','') }}美团</el-breadcrumb-item>
      <el-breadcrumb-item><a href="/">{{ city.replace('市','') }}{{ decodeURIComponent(keyword) }}</a></el-breadcrumb-item>
    </el-breadcrumb>
  </div>
</template>

<script>
export default {
  data() {
    return {
      city: '北京市'
    }
  },
  props: {
    keyword: {
      type: String,
      default: ''
    }
  }
}
</script>
