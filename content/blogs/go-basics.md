---
date: '2025-04-03T01:07:43+04:00'
draft: false
title: 'Go Basics: Variables, Types, and Strings'
tags: ["Go", "Golang", "Tutorial", "Basics", "Variables", "Types", "Strings"]
categories: ["Go Basics"]
description: ""
comments: true
---

### How's it going yall. Lets learn Go's basics today!

Alright, let's dive into the absolute basics of Go! Think of this as your "Level 1" - getting comfy with the fundamentals. No scary stuff, promise!

### Variables & Constants: The Building Blocks

First up, variables. In Go, you gotta declare 'em before you use 'em. Use the `var` keyword, give it a name, and tell Go what *type* it is[cite: 9, 21].

```go
// Declare an integer (Go has different sizes like int8, int16, int32, int64)
var varInt int16 = 12

// Unsigned int - only positive numbers, but can hold bigger values!
var intNum uint16

// Floats need a size too (float32 or float64)
var floatNum float32 = 123456.9567 // Might lose some precision
var float64Num float64 = 123456.9567 // More precise

fmt.Println(varInt)   // Output: 12
fmt.Println(float64Num) // Output: 123456.9567
```
<mark style="background-color:rgb(221, 195, 140); color: #000;">**Key Point:**</mark> Go is strict! If you declare a variable, you have to use it. Keeps the code clean, no pointless variables hanging around. Also, you can't mix types in operations directly (like adding an int and a float32) without converting first.

- You can also let Go figure out the type using := (short assignment statement) - super handy!

```go
myVar := "text" // Go knows this is a string
fmt.Println(myVar)
```
### Strings:
Strings are sequences of characters. Use double quotes "" for regular strings or backticks `` if you want Go to keep the exact formatting (like line breaks).

```go
var myString string = "Hello there!"
var multiLineString string = `This string
will keep its
line breaks.`

fmt.Println(myString)
fmt.Println(multiLineString)
```
Go strings are actually sequences of bytes, usually using UTF-8 encoding. We'll dig into that more later, but for now, just know they can hold pretty much any character!

### Quick Peek: Booleans
- Simple true/false stuff.

```go
var isCool bool = true
fmt.Println(isCool) // Output: true
```

### That's Wrap for Level 1!