# Portfolio:
a set of projects to show of how cool i am ✨✨

Take a look at my [Resume](resume.pdf)!
Here youl find my up to date work experience, interests, and more usefull info.

### lets start simple: fizzbuzz
``` rust
fn fizzbuzz (runtime: i32) {
    for iter in 1..=runtime {
        if iter % 3 == 0 && iter % 5 == 0 {
            println!("fizzbuzz")
        } else if iter % 3 == 0 {
            println!("fizz");
        } else if iter % 5 == 0 {
            println!("buzz")
        } else {
            println!("{iter}")
        }
    }
}
```

### fibinacci by index
``` rust 
fn fib_by_index(position: i32) -> i64 {
    let mut prev_prev = 0;
    let mut prev = 1;
    let mut now = 0;
    for iter in 0..position {
        now = prev_prev + prev;
        println!("{now}");
        prev_prev = prev;
        prev = now;
    }
    now
}
```
