# libwit

`libwit` is a small library that makes it easy to integrate Wit.ai with many programming languages. It manages client audio recording and communication with Wit.ai.

To compile as a Rust library, run

```bash
cargo build
```

To compile the C-compatible library, run

```bash
./build_c.sh
```

This will create a `libwit.a` file in the `lib` folder. You can use it in your C-compatible projects, along with the `include/wit.h` file.

To compile the example, run

```bash
cd example
gcc -Wall -o test test.c -I ../include -L ../lib -lwit -lsox -lcurl
```
