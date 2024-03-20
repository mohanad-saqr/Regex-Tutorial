# Understanding Regular Expressions: Email Validation

## Introduction

Regular Expressions (regex) are powerful tools used in programming for searching, matching, and manipulating text. This tutorial focuses on understanding how regex works through the lens of a commonly applied example: email validation. Email addresses follow a standard format that can be checked using regex, making this a perfect case study for our exploration.

## Summary

This tutorial breaks down the regex pattern `^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$`, which is used to validate email addresses. By understanding each component, you'll gain insights into regex's functionality and how it applies to real-world scenarios.

## Table of Contents

1. [Start of the String](#start-of-the-string)
2. [Username](#username)
3. [At Symbol (@)](#at-symbol-)
4. [Domain Name](#domain-name)
5. [Dot (.)](#dot-)
6. [Top-Level Domain](#top-level-domain)
7. [End of the String](#end-of-the-string)
8. [Author](#author)

## Start of the String

The `^` symbol matches the start of a string. It ensures that the regex pattern only matches from the beginning of the text.

## Username

`[a-zA-Z0-9._%+-]+` matches the username part of the email. This portion:
- Can contain letters (`a-zA-Z`), numbers (`0-9`), dots (`.`), underscores (`_`), percent signs (`%`), plus signs (`+`), and hyphens (`-`).
- The `+` ensures that one or more of the allowed characters are present.

## At Symbol (@)

The `@` character is literal and matches itself. It separates the username from the domain name in an email address.

## Domain Name

`[a-zA-Z0-9.-]+` matches the domain part of the email, which:
- Can include letters, numbers, dots, and hyphens.
- The `+` indicates that one or more of these characters must be present.

## Dot (.)

`\.` matches a literal dot character. It separates the domain and the top-level domain (TLD) in the email address.

## Top-Level Domain

`[a-zA-Z]{2,}` matches the top-level domain (TLD) of the email:
- Must consist of at least two letters (`{2,}`), with no upper limit on length.
- Represents domain categories like `.com`, `.org`, etc.

## End of the String

The `$` symbol matches the end of a string. It ensures that the regex pattern matches only if the entire string conforms to the email format.

## Author

This tutorial was created to help web development students understand and apply regex patterns. For more tutorials and coding tips, visit my [GitHub profile]https://github.com/mohanad-saqr

---

Remember, practice makes perfect. Try creating your own regex patterns and testing them against different inputs to see how they behave. Happy coding!

