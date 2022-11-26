# TypeScript

对象转类型

```ts
interface Map {
  'DAY':'日'
  'WEEK':'周'
  'MONTH':'月'
}
type MapType = keyof typeof Map
```

数组转类型

```ts
const OPTIONS = [
  {
    label: '日',
    value: 'DAY'
  },
  {
    label: '周',
    value: 'DAY'
  },
  {
    label: '月',
    value: 'DAY'
  }
]
type OptionType = (typeof OPTIONS)[number]['label']
```