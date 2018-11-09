<template>
  <div>
    <Form ref="formValidate" :label-width="90">
      <Card :bordered="false">
        <p slot="title">一列</p>
        <FormItem label="单行文本">
          <Input placeholder="Enter text"></Input>
        </FormItem>
        <FormItem label="多行文本">
          <Input type="textarea" :autosize="{minRows: 3,maxRows: 5}" placeholder="Enter something..."></Input>
        </FormItem>
      </Card>
      <Card :bordered="false">
        <p slot="title">两列</p>
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
          <FormItem label="单选">
            <RadioGroup>
              <Radio label="金斑蝶"></Radio>
              <Radio label="爪哇犀牛"></Radio>
              <Radio label="印度黑羚"></Radio>
            </RadioGroup>
          </FormItem>
          </Col>
          <Col span="12">
          <FormItem label="多选 ">
            <CheckboxGroup v-model="disabledGroup">
              <Checkbox label="香蕉"></Checkbox>
              <Checkbox label="苹果"></Checkbox>
              <Checkbox label="西瓜"></Checkbox>
            </CheckboxGroup>
          </FormItem>
          </Col>
        </Row>
      </Card>
      <Card :bordered="false">
        <p slot="title">三列</p>
        <Row>
          <Col span="8">
          <FormItem label="日期单选">
            <DatePicker type="date" placeholder="Select date" style="width: 100%;"></DatePicker>
          </FormItem>
          </Col>
          <Col span="8">
          <FormItem label="日期范围">
            <DatePicker type="daterange" placement="bottom-end" placeholder="Select date" style="width: 100%;"></DatePicker>
          </FormItem>
          </Col>
          <Col span="8">
          <FormItem label="选择单个时间">
            <TimePicker type="time" placeholder="Select time" style="width: 100%"></TimePicker>
          </FormItem>
          </Col>
        </Row>
        <Row>
          <Col span="8">
          <FormItem label="日期单选">
            <DatePicker type="date" placeholder="Select date" style="width: 100%;"></DatePicker>
          </FormItem>
          </Col>
          <Col span="8">
          <FormItem label="日期范围">
            <DatePicker type="daterange" placement="bottom-end" placeholder="Select date" style="width: 100%;"></DatePicker>
          </FormItem>
          </Col>
          <Col span="8">
          <FormItem label="选择单个时间">
            <TimePicker type="time" placeholder="Select time" style="width: 100%"></TimePicker>
          </FormItem>
          </Col>
        </Row>
      </Card>
      <Card :bordered="false">
        <p slot="title">四列</p>
        <Row>
          <Col span="6">
          <FormItem label="文本">
            <Input v-model="formValidate.name" placeholder="Enter text"></Input>
          </FormItem>
          </Col>
          <Col span="6">
          <FormItem label="文本">
            <Input v-model="formValidate.name" placeholder="Enter text"></Input>
          </FormItem>
          </Col>
          <Col span="6">
          <FormItem label="文本">
            <Input v-model="formValidate.name" placeholder="Enter text"></Input>
          </FormItem>
          </Col>
          <Col span="6">
          <FormItem label="文本">
            <Input v-model="formValidate.name" placeholder="Enter text"></Input>
          </FormItem>
          </Col>
        </Row>
        <Row>
          <Col span="6">
          <FormItem label="文本">
            <Input v-model="formValidate.name" placeholder="Enter text"></Input>
          </FormItem>
          </Col>
          <Col span="6">
          <FormItem label="文本">
            <Input v-model="formValidate.name" placeholder="Enter text"></Input>
          </FormItem>
          </Col>
          <Col span="6">
          <FormItem label="文本">
            <Input v-model="formValidate.name" placeholder="Enter text"></Input>
          </FormItem>
          </Col>
          <Col span="6">
          <FormItem label="文本">
            <Input v-model="formValidate.name" placeholder="Enter text"></Input>
          </FormItem>
          </Col>
        </Row>
      </Card>
    </Form>
  </div>
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