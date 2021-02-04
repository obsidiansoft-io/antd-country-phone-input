# antd-country-phone-input

Country phone input component as standard Ant.Design form item.

Currently only support Chinese.

![Preview](asset/screenshot.png)

## Installation

```
npm i @obsidiansoft/antd-country-phone-input
```

## [Usage](src/App.tsx)

[![Edit antd-country-phone-input](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/antd-country-phone-input-mtksn?fontsize=14)

```js
import { Button, Form } from 'antd';
import CountryPhoneInput from "antd-country-phone-input";

const App = () => {
  const onFinish = (values) => {
    console.log('Success:', values);
  };

  const onFinishFailed = (errorInfo) => {
    console.log('Failed:', errorInfo);
  };

  return (
    <Form
      onFinish={onFinish}
      onFinishFailed={onFinishFailed}
      style={{ width: 400, height: 300, margin: 40 }}
    >
      <Form.Item name="phone">
        <CountryPhoneInput />
      </Form.Item>
      <Form.Item>
        <Button type="primary" htmlType="submit">
          Submit
        </Button>
      </Form.Item>
    </Form>
  );
};

export default App;
```
