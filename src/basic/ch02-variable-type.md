# 變數與型別

## 變數宣告

`let <變數名稱>: <型別> = <值>;`

型別預設不可變(immutable)，若要變更變數值，需加上 mut 關鍵字。

`let mut <變數名稱>: <型別> = <值>;`

使用 const 取代 let 宣告常數(constant)。 通常用大寫字(Uppercase)母命名。

常數會在編譯期間被賦值，且一定要指定型別。

```rust,icon=.devicon-rust-plain
fn print_type_of<T>(_: &T) {
    println!("{}", std::any::type_name::<T>())
}

fn main() {
    let x1 = 100;
    println!("{x1}");
    println!("x1={x1}");

    let x2 = 200;
    println!("x2={x2}");
    println!("x2={x2:?}");

    let x3 = "300";
    println!("x3={x3}");
    println!("x3={x3:?}"); // 輸出時額外顯示字串引號

    print_type_of(&x1);

    let mut x4 = 400; // 可變
    println!("x4={x4}");
    x4 = 401;
    println!("x4={x4}");

    let mut x1 = x1; // 重新改成可變
    x1 += 1;
    println!("x1={x1}");

    let x4 = x4; // 重新改成不可變
    println!("x4={x4}");

    const YEAR: i32 = 2024; // 常數
    println!("{YEAR}");
}
```
