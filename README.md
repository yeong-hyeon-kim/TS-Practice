# π νλ‘μ νΈ κ°μ(Introduce Project)

## TS-Practice

* μμ λ‘ TypeScriptλ₯Ό μμλ΄λλ€.

## π‘ νμ μ€ν¬λ¦½νΈ(TypeScript)?

* νμμ€ν¬λ¦½νΈ(TypeScript)λ μλ°μ€ν¬λ¦½νΈ(JavaScript)μ νμ₯ λ²μ  μλλ€.
* μλ°μ€ν¬λ¦½νΈ(JavaScript)μ λ¬λ¦¬ νμ(Type)μ€ν¬λ¦½νΈ(Script) μ΄λ¦ κ·Έλλ‘ μ μ  νμμ λͺμν  μ μμ΅λλ€.
* λμ  νμμ μ¬μ©νλ μλ°μ€ν¬λ¦½νΈ(JavaScript)μμ λ°μν  μ μλ νμ μλ¬λ€μ μ μ  νμ μ¬μ©μΌλ‘ λ―Έλ¦¬ μ‘λ κ²μ΄ νμμ€ν¬λ¦½νΈ(TypeScript)μ μ£Όλ λͺ©μ μλλ€.
* μλ°μ€ν¬λ¦½νΈ(JavaScript)
  * `"μ½λ μ΄λ»κ²λ  μ€νμν¬κ»~ λ€λ§ λ¬Έμ κ° μλ€λ κ±΄ λ³΄μ₯ν  μ μμ΄..."`

* νμμ€ν¬λ¦½νΈ(TypeScript)
  * `"μ΄ λΆλΆ λ¬Έμ  μμΌλκΉ ν΄κ²°νκ³  μ€νν  ν  μ μμ΄ μμ νλ©΄ μ΄ λΆλΆμ λ¬Έμ  μμ΄ μ€νν  μ μμ΄!"`

### κΈ°λ³Έ νμ(Basic Type)

* μλ°μ€ν¬λ¦½νΈ κΈ°λ³Έ νμμ νμμ€ν¬λ¦½νΈλ‘ ννν©λλ€.

```typescript
// λ¬Έμμ΄ νμ : String Type.
const message: string = "Hello World";
// μ«μ νμ : Number Array Type.
const numbers: number[] = [1, 2, 3];
// λ¬Έμμ΄ λ°°μ΄ νμ : String Array Type.
const messages: string[] = ["Hello", "World"];
// λΌλ¦¬ κ° νμ : TureFalse boolean Type.
const TrueFalse: boolean = false;

// μ‘°κ±΄λ¬Έμμ OR μ°μ°μλ₯Ό '||' μΌλ‘ νννλ κ²κ³Ό λΉμ·ν©λλ€.
// Number Or Null Type.
let NumberOrNull: number | null = null;
// String Or Undefined Type.
let StringOrUndefined: string | undefined = undefined;
// Value Type.
let Energy: "Oil" | "Gas" | "Hydrogen" | "Atomic" | "Coal" | "Water";
```

### ν¨μ νμ(Function Type)

* μλ°μ€ν¬λ¦½νΈ ν¨μλ₯Ό νμμ€ν¬λ¦½νΈλ‘ ννν©λλ€.

```typescript
// function AnyFunc(λ§€κ° λ³μ : νμ) : number(λ°ν νμ)
function Sum(x: number, y: number) : number{
  return x + y;
}

Sum(1, 2);

// λ°ν νμμ΄ μμ κ²½μ° void
function PrintSum(x: number, y: number): void {
  console.log(x + y);
}

PrintSum(1, 2);
```

### μ λ€λ¦­(Generics)

* μ¬λ¬ νμμ λνμ¬ νΈνμ λ§μΆ°μΌ νλ μν©μμ μ¬μ©νλ λ¬Έλ²μλλ€.
* μ μΈ μ νμμ μ§μ νμ§ μκ³  μ¬μ© μ νμμ μ§μ ν©λλ€.

```typescript
function wrap<T>(param: T) {
  return {
    param,
  };
}

interface Items<T> {
  list: T[];
}

const items: Items<string> = {
  list: ["a", "b", "c"],
};

```

## π» κ°λ° νκ²½(Develop Environment)

### μΈλΆ νκ²½(Environment Detail)

||μ΄μμ²΄μ (OS)|μΈμ΄(Language)|νλ μμν¬(Framework)|
|-|:-:|:-:|:-:|
|λͺμΉ­(Name)|![Windows](https://img.shields.io/badge/Windows-0078D6?style=flat-square&logo=Windows&logoColor=white)|![TYPESCRIPT](https://img.shields.io/badge/TYPESCRIPT-3178C6?style=flat-square&logo=TypeScript&logoColor=white)|![NODE](https://img.shields.io/badge/NODE.JS-339933?style=flat-square&logo=Node.js&logoColor=white)|
|λ²μ (Version)|`10, 11`|`4.7.4`|`18.6.0`|

## π λΉκ³ (Remark)

* NPM(Node Package Manager) μ΄κΈ°ν : `npm init -y`
* νμμ€ν¬λ¦½νΈ(TypeScript) ν¨ν€μ§ μ€μΉ : `npm i -g typescript`
* νμμ€ν¬λ¦½νΈ νκ²½μ€μ  : `tsc --init`
  * [tsconfig.json](./tsconfig.json)
* νμμ€ν¬λ¦½νΈ μ»΄νμΌ(Compile) :  `tsc`
* νμμ€ν¬λ¦½νΈ μ€ν : `node` [src/practice](./src/practice.ts)
