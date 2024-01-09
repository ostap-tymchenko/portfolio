# Portfolio:
<!-- a set of projects to show of how cool i am ✨✨ -->
<img src="https://github-readme-streak-stats.herokuapp.com/?user=ostap-tymchenko&theme=rose&hide_border=true&mode=weekly" alt="ostap-tymchenko"/>


<button id="close" class="closing" onClick="javascript:close_clip()"><img width="100px" hight="100px" src="pdf-icon.png"/></button>
<button id="close" class="closing" onClick="javascript:close_clip()"><img src="leetcode-icon.png"/></button>
<p>Resume&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Leetcode</p>

<style>
.fcc-btn {
	color: white;
	padding: 35px 35px;
	text-decoration: none;
}

img {
    width: 200px;
    height: 200px;
}
</style>

#### Fizzbuzz
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

#### Fizzbuzz by match, simpler sintax, more extendable

``` rust
fn fizzbuzz_with_match (runtime: i32) {
    for iter in 1..=runtime {
        match (iter % 3 , iter % 5) {
        (0, 0) => println!("fizzbuzz"),
        (0, _) => println!("fizz"),
        (_, 0) => println!("buzz"),
        _ => println!("{iter}"),
        }
    }
}
```

#### Fibonacci by index (Significantly more performant than recursive solution)
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
