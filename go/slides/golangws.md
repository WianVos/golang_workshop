# Go!!

![Gopher](https://www.hardwinsoftware.com/blog/wp-content/uploads/2018/02/golang-gopher.png) <!-- .element height="50%" width="50%" -->


---



## started in 2009 
## by Robert Griesemer, Rob Pike, and Ken Thompson

## @GOOGLE

---

# Key Selling points

- statically typed
- (cross) compiles to binary (no installed runtime needed)
- Fast!!

---

# Used by:

- Docker
- Kubernetes
- Minio
- .......

---

##### static vs. Dynamic

Short explaination: 

statically typed languages need to know the type of a variable at compile time dynamically typed languages do not

---

## Languages by type
<section>
  <div style="text-align: center; float: left;border: 3; background: None">
    <h3 data-markdown>Static</h3>
    <p data-markdown>java</p>
    <p data-markdown>c++</p>
    <p data-markdown>Rust</p>
    <p data-markdown>GO</p>
    <!-- more Elements -->
  </div>
  <div style="text-align: center; float: right;">
    <h3 data-markdown>Dynamic</h3>
    <p data-markdown>Python</p>
    <p data-markdown>Ruby</p>
    <p data-markdown>Perl</p>
    <!-- more Elements -->
  </div>
</section>

---

### **Stuff you need to know** 

 




* Go is object oriented, but.... 
* A running programm starts with a main.go function from package main (we'll get to that)
* Go has a great multi-threading system (maybe we'll get to that.. if ur nice)
* Go is very picky ... try assigning a variable an not use it .. 

---
### Hello World

```golang
package main

import (
    "fmt"
    )

func main() {
    fmt.Println("Hello World!!")
}
```
[https://play.golang.org/p/HmnNoBf0p1z]

---
### variables

declaration methods
* var keyword (returns a variable initialized with its zero value)
* := short variable declaration

---

### variables

```golang
    //keyword initialization
    var x string
    var y int
    var z bool

    // init and set value
    var x = "hello world" 

    //short variable declaration
    a, b, c := 10, "hello world", true

```

[https://play.golang.org/p/K5SPD69WUn0]


---


### slices/arrays

!! this is in no way enough to grasp the full concept !!
But here's the 20/80 version
```golang

 var x []string  // declaring a slice of strings
 var x []int    // declaring a slice of ints
 var x = []string{"a", "b" , "c" }  // declaring a new slice and initializing it with some Elements
 
 ```
[https://play.golang.org/p/3VjWdQwAZ_F]
[https://play.golang.org/p/cFkuVKVfECJ]


---

### maps

Maps are used to store key value pairs

```golang

 var x map[string]string  // declaring map where both key and value are strings
 var x map[string]int    // declaring a map where the key is a string and the value is an integer
 var x = map[string]string{{"a": "b"} ,{ "c": "d"} }  // declaring a new slice and initializing it with some Elements
 
 ```

[https://play.golang.org/p/k0IPdxaKwZx]
[https://play.golang.org/p/t_YmokMMeyq]


---

### If statement

```golang
if x == "" {
    fmt.Println("x is empty")
} else if x == "dr steven strange" {
    fmt.Println("hello dr strange")
}else{
    fmt.Println("x is definitively not empty")
}

```
[https://play.golang.org/p/823avjk3Y1m]
[https://play.golang.org/p/UulXs48eHF3]


---

### functions

functions in golang are not very difficult to understand 

```golang

func thisIsAPrivateFunction(a string, b,c int) (string){
   return  fmt.Sprintf("%s is a string, %d and %d are integers", a,b,c )
}
```

[https://play.golang.org/p/LycAapUYtku]
[https://play.golang.org/p/ibBCcTizfqA]


---

### object orientation


It's all about the data ... 
Yes go is obejct oriented .. no there is no class .. 
None... no need .. 

we have structs .. 

```golang
type fiets struct{
    wielen int
    trappers int
    merk string
}
```

Let me demonstrate

[https://play.golang.org/p/pZPPgRKs9Bw]
[https://play.golang.org/p/OB4H1OGOsYW]

---

### variable scoping

In Go variables have a scope .. 

scopes are:
package 
function
if / switch / for 

[https://play.golang.org/p/csJ8zg60xKS]

---


### Pointers

!! Pay attention .. this stuff is important !!

golang has two ways of passing a variable .. 
either by reference or by value .. 

[https://play.golang.org/p/yMUJ53UDSDc]


---

### goroutines

Goroutines: multithreading made easy 


[https://play.golang.org/p/4zQRzXAZXdC]


---


### Channels

channels .. it's a thing .. and we need to talk about it 

[https://play.golang.org/p/stTN2ZfBGp_s]