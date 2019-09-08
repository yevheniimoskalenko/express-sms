<template>
  <el-row>
    <el-col :span="24">
      <el-form ref="form" v-model="form" :inline="true">
        <el-form-item label="Service">
          <el-input v-model="form.service" />
        </el-form-item>
        <el-button type="primary" :loading="loading" round>Поиск</el-button>
      </el-form>
    </el-col>
  </el-row>
</template>

<script>
export default {
  data() {
    return {
      loading: false,
      form: {
        service: ""
      }
    };
  }
};
</script>
