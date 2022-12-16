# rehype-sectionize

![test workflow](https://github.com/hbsnow/rehype-sectionize/actions/workflows/test.yml/badge.svg)

## Motivation

There is already [rehype-section](https://github.com/agentofuser/rehype-section) in the library for sectioning. But it could not change the class of section. I was referred [rehype-section](https://github.com/agentofuser/rehype-section). Thanks.

## Install

```
npm i -D @hbsnow/rehype-sectionize
```

## Sample

### Input

```html
<h1>h1</h1>
<h2>h2</h2>
<h3>h3</h3>
```

### Output

```html
<section class="heading" data-heading-rank="1">
  <h1>h1</h1>
  <section class="heading" data-heading-rank="2">
    <h2>h2</h2>
    <section class="heading" data-heading-rank="3">
      <h3>h3</h3>
    </section>
  </section>
</section>
```

## Options

| option              | type                    | default     | description                    |
| ------------------- | ----------------------- | ----------- | ------------------------------ |
| `properties`        | `hastscript.Properties` | `undefined` | Attributes assigned to section |
| `enableRootSection` | `boolean`               | `false`     | Section to wrap all            |

## License

[MIT][license] © [hbsnow][author]