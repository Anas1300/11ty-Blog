---
title: Like everything needs to be secured
author: Anas Ahmed
date: 2021-06-27
image: /assets/blog/article-.png
imageAlt: this is a test
description: A conversation I was having with my parents about what to do in life and thinking about it in retrospection
---

## 🚩 Introduction

Hell yeah, that would be cool. 😎 So this is gonna be about **fine-tuning your css** designs in a manner that would make your **pages load faster** 🚀 as well as make your designs all **browser compatible**. 💻 And by all means, make your CSS production ready for getting the best out of your CSS. 🎉

Yes, the above image is from the console and you can customize the text however you like. To know how keep reading till the end.

It's been a while since my last post, it's because I got into learning some interesting stuff and undoubtedly writer's block was back. But recently, while working on a large repository that had a lot of stuff logged in the console I wanted a way to clear all the clutter and make my console statements stand out from the rest.

Here is how I was able to do that and how you could too.

So these are the possible options:

- Using different console methods
- Using various format specifiers (believe me, this is magic ✨)


## Using different console methods

You might already know some of the basic ones, like:

- console.log
- console.info
- console.error
- console.warn

## console.table

This can be used to log large nested objects or arrays so you don't have to go through expanding each key to view the whole thing.

```javascript
let peoples = [
  {
    name: "Richard Hendricks",
    location: "Berkely",
    cell: "4254-024-8162",
    age: 32,
  },
  {
    name: "Christiansen Frederikke",
    location: "Madras",
    cell: "4987-024-2562",
    age: 34,
  },
  {
    name: "John Doe",
    location: "California",
    cell: "3143-344-342",
    age: 53,
  },
];

console.table(peoples);
```

## console.group and console.groupEnd

You can group a set of console logs having a particular meaning apart from the rest using this method.

```javascript
const title = "Me and my boys";

console.group(title);
console.table(peoples[0]);
console.info("Weather is very beautiful today ☁");
console.warn("Don't fall for the beautiful weather");
console.groupEnd(title);
```

## Using format specifiers

Believe it or not, console logs can be more than just simple messages. You can include an eye-catching message or something more convincing as your favorite dog image.

All because you can use format specifiers inside them. How?

## List of available format specifiers

- %s ⇒ Formats as string
- %i ⇒ Formats as integer
- %f ⇒ Formats as float
- %O ⇒ Formats as object (yes that's capital O as in Oregano)
- %o ⇒ Formats as DOM element
- %c ⇒ Formats as CSS ✨


## Formats as string, integer, float

```javascript
console.log(
  "%s, told me that we're going to mall today with %s",
  "Alan",
  "Mike"
);
// Alan, told me that we're going to mall today with Mike

console.log("We had %i mangoes today", 56);
// We had 56 mangoes today

console.log(
  "Did you know, Tesla Model S can reach 0 to 60 mph in %f seconds?",
  2.3
);
// Did you know, Tesla Model S can reach 0 to 60 mph in 2.3 seconds?
```

That's it, super easy! 😃

## 🤝Conclusion

For me, all that mattered was for the logs to stand out and be more catchy on pursuit of which I found out a ton of more cool stuff we can do, hope this gives you more clarity on the gem of a function, that console is.
