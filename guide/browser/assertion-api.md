---
title: Assertion API | Browser Mode
---

# Assertion API

Vitest 捆绑了 [`@testing-library/jest-dom`](https://github.com/testing-library/jest-dom)库，以提供各种开箱即用的 DOM 断言。有关详细文档，请阅读 `jest-dom` readme：

- [`toBeDisabled`](https://github.com/testing-library/jest-dom#toBeDisabled)
- [`toBeEnabled`](https://github.com/testing-library/jest-dom#toBeEnabled)
- [`toBeEmptyDOMElement`](https://github.com/testing-library/jest-dom#toBeEmptyDOMElement)
- [`toBeInTheDocument`](https://github.com/testing-library/jest-dom#toBeInTheDocument)
- [`toBeInvalid`](https://github.com/testing-library/jest-dom#toBeInvalid)
- [`toBeRequired`](https://github.com/testing-library/jest-dom#toBeRequired)
- [`toBeValid`](https://github.com/testing-library/jest-dom#toBeValid)
- [`toBeVisible`](https://github.com/testing-library/jest-dom#toBeVisible)
- [`toContainElement`](https://github.com/testing-library/jest-dom#toContainElement)
- [`toContainHTML`](https://github.com/testing-library/jest-dom#toContainHTML)
- [`toHaveAccessibleDescription`](https://github.com/testing-library/jest-dom#toHaveAccessibleDescription)
- [`toHaveAccessibleErrorMessage`](https://github.com/testing-library/jest-dom#toHaveAccessibleErrorMessage)
- [`toHaveAccessibleName`](https://github.com/testing-library/jest-dom#toHaveAccessibleName)
- [`toHaveAttribute`](https://github.com/testing-library/jest-dom#toHaveAttribute)
- [`toHaveClass`](https://github.com/testing-library/jest-dom#toHaveClass)
- [`toHaveFocus`](https://github.com/testing-library/jest-dom#toHaveFocus)
- [`toHaveFormValues`](https://github.com/testing-library/jest-dom#toHaveFormValues)
- [`toHaveStyle`](https://github.com/testing-library/jest-dom#toHaveStyle)
- [`toHaveTextContent`](https://github.com/testing-library/jest-dom#toHaveTextContent)
- [`toHaveValue`](https://github.com/testing-library/jest-dom#toHaveValue)
- [`toHaveDisplayValue`](https://github.com/testing-library/jest-dom#toHaveDisplayValue)
- [`toBeChecked`](https://github.com/testing-library/jest-dom#toBeChecked)
- [`toBePartiallyChecked`](https://github.com/testing-library/jest-dom#toBePartiallyChecked)
- [`toHaveRole`](https://github.com/testing-library/jest-dom#toHaveRole)
- [`toHaveErrorMessage`](https://github.com/testing-library/jest-dom#toHaveErrorMessage)

如果使用 TypeScript 或希望在 `expect` 中获得正确的类型提示，请确保根据使用的提供程序，在 `tsconfig` 中指定了 `@vitest/browser/providers/playwright` 或 `@vitest/browser/providers/webdriverio`。如果使用默认的 `preview` 提供程序，则可指定 `@vitest/browser/matchers` 代替。

::: code-group
```json [preview]
{
  "compilerOptions": {
    "types": [
      "@vitest/browser/matchers"
    ]
  }
}
```
```json [playwright]
{
  "compilerOptions": {
    "types": [
      "@vitest/browser/providers/playwright"
    ]
  }
}
```
```json [webdriverio]
{
  "compilerOptions": {
    "types": [
      "@vitest/browser/providers/webdriverio"
    ]
  }
}
```
:::
