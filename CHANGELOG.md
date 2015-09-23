Changelog
=========

> **Tags:**
> - [New Feature]
> - [Bug Fix]
> - [Documentation]
> - [Internal]
> - [Polish]

## 2.0.1

- **New Feature**
  - Throw an compile-time error when there is an unused JSX Element.
    - Before, these would be silently removed from the output.
- **Bug Fix**
  - Properly detect the whether the current JSX Element is the "root"
    element of the render function.
    - Before, any JSX Element that appeared laster in the same file
      would be "root". Now, only elements that appear later in the
      current function or it's contianing functions are roots.
- [Internal]
  - Test that compile-errors are thrown.

## 2.0.0

- **New Feature**
  - Support rendering arbitrary children expressions:
    1. "Textual" expressions, including numbers and strings.
    2. Other JSX Elements.
    3. Arrays or Objects containing #1, #2, or #3.
  - Throw an compile-time error when using JSX Namespaces.
- **Internal**
  - A massive rewrite to support full JSX compatibility.

## 1.X

- Initial implementation.