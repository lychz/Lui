### 基本用法

```jsx
<Switch onChange={v => console.log(v)}></Switch>
```

### 设置选中/未选中显示的内容

```jsx
<Switch checkedChildren={"checked"} unCheckedChildren={"unchecked"}></Switch>
```

### 默认选中
```jsx
<Switch defaultValue></Switch>
```

### 禁用状态

```jsx
<Switch disabled></Switch>
```

### 受控组件

```jsx
import Button from "@components/Button";
import { useState } from "react";
const [value, setChecked] = useState(false)
const change = () => {
  setChecked(!value)
}

<div>
  <Switch defaultValue value={value}></Switch>
  <br />
  <br />
  <Button onClick={change}>switch</Button>
</div>

```
