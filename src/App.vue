<template>
  <Button theme="link">1123</Button>
  <Switch v-model:value="value"></Switch>
  <Layout>
    <Header>header</Header>
    <Content>content</Content>
    <Footer>footer</Footer>
  </Layout>
  <Input v-model:value="value1" placeholder="请输入内容" />
  <Input :value="value1" />

  <Tabs v-model:selected="x">
    <Tab title="导航一">内容一</Tab>
    <Tab title="导航二">内容二</Tab>
    <Tab title="导航三">内容三。。。。。。。。。。。。</Tab>
  </Tabs>
</template>

<script lang="ts">
import {
  Switch,
  Button,
  Tabs,
  Tab,
  Dialog,
  Input,
  Layout,
  Header,
  Content,
  Footer,
  Aside,
} from "language-ui-1";
import "language-ui-1/dist/lib/language.css";
export default {
  name: "App",
  data() {
    return {
      value: false,
      value1: null,
      x: "导航二",
    };
  },
  components: {
    Switch,
    Button,
    Tabs,
    Tab,
    Dialog,
    Input,
    Layout,
    Header,
    Content,
    Footer,
    Aside,
  },
};
</script>

<style></style>
