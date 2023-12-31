## Thread_TCP_Check CLI - Multiple Hosts using Rust

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li><a href="#installing-rust">Installing Rust</a></li>
    <li><a href="#build">Build</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#using-example">Using Example</a></li>
  </ol>
</details>

## About
Using Rust to Build CLI Application to Check Socket Connection of Multiple Hosts by Thread Mode 

## Installing Rust
If you’re running macOS, Linux, or another Unix-like OS.
To download Rustup and install Rust, run the following in your terminal, then follow the on-screen instructions.

```sh
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

## Build

```sh
git clone https://github.com/andrealvesguimaraes/thread-tcp-check.git
cd thread-tcp-check
cargo build --release
```


### Edit Hosts to Test
```sh
nano iplist.txt
```

## Usage

Usage: thread-tcp-check [OPTIONS] 
<pre>
Options:

   -f, --file      File Name

   -p, --port      TCP Port Number

   -h, --help      Print Help  

   -V, --version   Print Version
</pre>

## Using Example
```sh
./target/release/thread-tcp-check --file iplist.txt --port 8080
```
