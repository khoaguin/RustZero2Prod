## Features
We will fulfill two user stories:
- As a blog visitor,
    - I want to subscribe to the newsletter, so that I can receive email updates when new content is published on the blog;
- As the blog author,
    - I want to send an email to all my subscribers, so that I can notify them when new content is published.

We will not add features to
- unsubscribe;
- manage multiple newsletters;
- segment subscribers in multiple audiences;
- track opening and click rates.


## Dev Tools
- We use `cargo watch` to automate the process of checking, testing, and running your code whenever changes are detected: `cargo install cargo-watch`.  
Run `cargo watch -x check -x test -x run` to start a process that monitor changes in your code. Whenever there is a change, it will run `cargo check`. If that succeeds, it launches `cargo test`. If tests pass, it launches the application with `cargo run`

- We use `tarpaulin` for code coverage: `cargo install cargo-tarpaulin`. Run `cargo tarpaulin --ignore-tests` to compute code coverage for your application code, ignoring your test functions

- We use `clippy` as linter: `rustup component add clippy`. Run `cargo clippy` to check your code for common mistakes and improve your code quality

- We use `rustfmt` for formatting: `rustup component add rustfmt`. Format the whole project with `cargo fmt`

- We use `audit` to check for code security vulnerabilities: `cargo install cargo-audit`. Run `cargo audit` to check for vulnerabilities in your dependencies