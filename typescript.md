# TypeScript

枚举转类型

```ts
enum CycleEnum {
  'DAY':'日'
  'WEEK':'周'
  'MONTH':'月'
}
type CycleType = keyof typeof CycleEnum
```

数组转类型

```ts
const CYCLE_OPTIONS = [
  {
    label: '日',
    value: 'DAY'
  },
  {
    label: '周',
    value: 'WEEK'
  },
  {
    label: '月',
    value: 'MONTH'
  }
] as const
type CycleType = (typeof CYCLE_OPTIONS)[number]['value']
```