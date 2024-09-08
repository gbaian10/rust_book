# Rust 基礎

* [官網](https://www.rust-lang.org/)
* [中文官網](https://www.rust-lang.org/zh-TW)

## 安裝 Rust

安裝

```bash,icon=.devicon-bash-plain
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

更新

```bash,icon=.devicon-bash-plain
rustup update
```

VSCode 安裝 Rust 插件

1. rust-analyzer
2. CodeLLDB

## Hello World(使用 rustc)

```rust,icon=.devicon-rust-plain
fn main() {
    println!("Hello, world!");
}
```

```bash,icon=.devicon-bash-plain
rutstc src/main.rs
```

會產生一個 `main` 或 `main.exe` 執行檔和一個 `main.pdb` 除錯輔助資訊檔

## 建立專案(使用 cargo)

* 使用 cargo 建立專案

```bash,icon=.devicon-bash-plain
cargo new hello_world
```

* 建置專案，會產生一個 `target` 資料夾

```bash,icon=.devicon-bash-plain
cd hello_world
cargo build
```

* 執行專案

```bash,icon=.devicon-bash-plain
cargo run
cargo run -q
```

* 清除專案

```bash,icon=.devicon-bash-plain
cargo clean
```

* 新增套件

```bash,icon=.devicon-bash-plain
cargo add <???>
```

---

* [Cargo Booke](https://doc.rust-lang.org/cargo/)
* [Build Commands](https://doc.rust-lang.org/cargo/commands/build-commands.html)
* [The Rust Programming Language](https://doc.rust-lang.org/book/)
* [Rust 程式設計語言](https://rust-lang.tw/book-tw/)
* [totorialspoint Rust](https://www.tutorialspoint.com/rust/index.htm)
* [awesome-rust](https://github.com/rust-unofficial/awesome-rust)
