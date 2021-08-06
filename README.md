# Regex-Tutorial


In this tutorial we will discuss about Regular Expressions which are known as Regex. We will discuss about what they are, what they are used for and a couple of examples for regex.

## Table of Contents

- [What is a Regex](#what-is-a-regex)
- [Email Regex Example](#email-regex-example)
- [The first forward slash](#The-first-forward-slash)
- [The special symbol](#The-special-symbol)
- [Username](#username)
- [The at symbol](#The-at-symbol)
- [Domain name](#domain-name)
- [Top-level domain name](#top-level-domain-name)
- [The dollar sign](#The-dollar-sign)
- [The last forward slash](#The-last-forward-slash)
- [About the author](#about-the-author)

## What is a Regex?

Regex is short form of “Regular Expressions”. A regex is a sequence of character which is used to search a specific pattern in the data. A regex search for a pattern in data and validates if the data is following a specific pattern. Regex are used for multiple purposes; they are used in search algorithms and for validation of input data. In search algorithms, they are used for “find” or “find and replace” actions whereas in validation, it determines whether an input is following a specific pattern or not.

## Email Regex Example

```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```
The example we chose for this tutorial is a regex which validates an email input. This regex searches for all the parts of email for example if we have this email abc@xyz.com then, it should look for the username ‘abc’, symbol ‘@’, second-level domain name `xyz`, a dot
`.` and a top-level domain name which in this case can be `com`.

## The first forward slash

```
/
```

The first component in the email regex is a forward slash `/`. This forward slash denotes the boundaries of a regular expression.

## The special symbol

```
^
```

The second component in the email regex is caret character ‘^’. It is also called as anchor tag ‘^’. This anchor tag means the string is starting from this time.
The first two characters of this regex are found in almost every regex because they show the boundary and start of expression.

## Username

```
([a-z0-9_\.-]+)
```

The next component in out selected regular expression is as above. This section of regex finds the username in the given data or a string.  The `()` brackets at the start and end of this component means that this component is a sub-expression of this complete regular expression. The a-z0-9 shows that it can have alphabets from a to z and numeric characters from 0 to 9. It also includes some characters after back slash `\.-`. In regular expressions any character after back slash means it should be found as it is in the expression. So this `\.-` means that the username can have a full stop `.` or dash `-` in the username.
All these components `a-z0-9\.-` are surrounded in a square bracket `[]` and it has a plus sign `+` next which indicates that there must be one or more characters in the username from this group of components.
The username which should match this sub-expression are `abc123`, `sara.abc` etc.

## The at symbol

```
@
```

The at symbol “@” after username section shows that there must be this symbol in the given input data.

## Domain name

```
([\da-z\.-]+)
```

The next sub-expression in our regex is as above. This sub-expression search for the domain name in the given input data after the username and the symbol. The first component in this part is `\d` this component search for numeric digits in the given input data. So this, is basically same as `0-9`. The next component is `a-z`, which means it can have alphabets from `a-z` and then we have `\.-` which means it can also have full stop and dash `-`.

This section also has square brackets around and a plus sign which means there must be one or more character from this section in the given input data.
The domain name which should match this sub-expression are ‘gmail’, ‘hotmail’, ‘outlook’ etc.

## Dot

```
.
```

The next component we have in our regex is ‘\.’. It means that there must be full stop after the domain name and before the next section.



## Top-level domain name

```
([a-z\.]{2,6})
```

The next sub-expression in our regex is as above. This sub-expression searches for the top-level domain name in the given input data. In this sub-expression we have `a-z\.` in the square brackets which means it can have alphabets and a full stop in the input data. This section does not have `\d` or `0-9` so, it can not have any numeric digits. The next thing after square brackets is a curly bracket with two numeric digits in them `{2,6}`. These curly brackets shows the number of characters this sub-expression can have and the digit between them shows minimum and maximum range. In this case we have 2 and 6 which means it can have at least 2 and utmost 6 characters in the top-level domain.
The top-level domain name which should match this expression are ‘com’, ‘org’, ‘edu’ etc.

## The dollar sign

```
$
```

The dollar sign in the regex shows that this is the end of a string.

## The last forward slash

```
/
```

The last forward slash in our regular expression shows the end boundary of input string. As there were a forward slash in the beginning which shows the starting boundary this slash shows the end boundary of the regular expression.

## About the author
I am BITENDELO LUBAISHA KANGA, student who likes to become web developer and web designer.

Please find my [github profile link](https://github.com/S0519).

© 2021, All rights reserved.






![Screenshot (207)](https://user-images.githubusercontent.com/80322588/126871811-937411ce-b5fd-4146-96f6-92aebd9327fb.png)



## URL

https://s0519.github.io/Regex-Tutorial/

