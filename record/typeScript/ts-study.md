# typeScript-全面进阶指南学习笔记


## 1.原始类型的类型标注 

> - 与 [JavaScript 数据类型和数据结构](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Data_structures#%E5%8E%9F%E5%A7%8B%E5%80%BC_primitive_values)  对应,在 TypeScript 中它们都有对应的类型注解。

```typeScript
    const name: string = 'mayunlong';
    const age: number = 24;
    const male: boolean = false;
    const undef: undefined = undefined;
    const nul: null = null;
    const obj: object = { name, age, male };
    const bigintVar1: bigint = 9007199254740991n;
    const bigintVar2: bigint = BigInt(9007199254740991);
    const symbolVar: symbol = Symbol('unique');
```

### null 与 undefined

> - `JavaScript` 中 `null` 与 `undefined` 分别表示 “这里有值，但是个空值” 和 “这里没有值” 。
> - `TypeScript` 中, `null` 与 `undefined` 类型都是有具体意义的类型。也就是说，它们作为类型时，表示的是一个有意义的具体类型值。这两者在没有开启 `strictNullChecks` 检查的情况下，会被视作其他类型的子类型，比如 `string` 类型会被认为包含了 `null` 与 `undefined` 类型：

```typeScript
	const tmp1: null = null;
	const tmp2: undefined = undefined;
	// 以下两个仅在关闭 strictNullChecks 时成立
	const tmp3: string = null;
	const tmp4: string = undefined;
```