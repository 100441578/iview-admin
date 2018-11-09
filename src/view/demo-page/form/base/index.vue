<template>
  <Card>
    <p slot="title">普通表单</p>
    <Form ref="formValidate" :label-width="90">
      <FormItem label="单行文本">
        <Input placeholder="Enter text"></Input>
      </FormItem>
      <FormItem label="多行文本">
        <Input type="textarea" :autosize="{minRows: 3,maxRows: 5}" placeholder="Enter something..."></Input>
      </FormItem>
      <Row>
        <Col span="12">
        <FormItem label="下拉单选">
          <Select placeholder="Select your city">
            <Option value="beijing">New York</Option>
            <Option value="shanghai">London</Option>
            <Option value="shenzhen">Sydney</Option>
          </Select>
        </FormItem>
        </Col>
        <Col span="12">
        <FormItem label="下拉多选">
          <Select multiple placeholder="Select citys">
            <Option value="beijing">New York</Option>
            <Option value="shanghai">London</Option>
            <Option value="shenzhen">Sydney</Option>
          </Select>
        </FormItem>
        </Col>
      </Row>
      <Row>
        <Col span="12">
        <FormItem label="日期单选">
          <DatePicker type="date" placeholder="Select date" style="width: 100%;"></DatePicker>
        </FormItem>
        </Col>
        <Col span="12">
        <FormItem label="日期范围">
          <DatePicker type="daterange" placement="bottom-end" placeholder="Select date" style="width: 100%;"></DatePicker>
        </FormItem>
        </Col>
      </Row>
      <Row>
        <Col span="12">
        <FormItem label="选择单个时间">
          <TimePicker type="time" placeholder="Select time" style="width: 100%"></TimePicker>
        </FormItem>
        </Col>
        <Col span="12">
        <FormItem label="选择范围时间">
          <TimePicker type="timerange" placement="bottom-end" placeholder="Select time" style="width: 100%"></TimePicker>
        </FormItem>
        </Col>
      </Row>
      <Row>
        <Col span="12">
        <FormItem label="单选">
          <RadioGroup>
            <Radio label="金斑蝶"></Radio>
            <Radio label="爪哇犀牛"></Radio>
            <Radio label="印度黑羚"></Radio>
          </RadioGroup>
        </FormItem>
        </Col>
        <Col span="12">
        <FormItem label="复选 ">
          <CheckboxGroup v-model="disabledGroup">
            <Checkbox label="香蕉"></Checkbox>
            <Checkbox label="苹果"></Checkbox>
            <Checkbox label="西瓜"></Checkbox>
          </CheckboxGroup>
        </FormItem>
        </Col>
      </Row>

      <FormItem>
        <Button type="primary">Submit</Button>
        <Button style="margin-left: 8px">Reset</Button>
      </FormItem>
    </Form>
  </Card>
</template>
<script>
  export default {
    data() {
      return {
        formValidate: {},
        ruleValidate: {}
      }
    },
    methods: {}
  }
</script>