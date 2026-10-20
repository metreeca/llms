# @metreeca/llms

[![npm](https://img.shields.io/npm/v/@metreeca/llms)](https://www.npmjs.com/package/@metreeca/llms)

AI tasks and shared services for [@metreeca/llms](https://github.com/metreeca/llms).

Provides primitives for working with embedding vectors from any model provider: condensing the fields of a resource into
the text to be embedded, ranking vectors by semantic proximity, and storing them in a compact textual form.

Jobs using them are set up and run under the [@metreeca/gear](https://github.com/metreeca/gear) job executor. This
package contributes building blocks for those jobs, not an execution runtime of its own.

# Installation

```shell
npm install @metreeca/gear  # the job executor
npm install @metreeca/llms  # this package
```

> [!IMPORTANT]
>
> Node.js 22 or later is required.

> [!WARNING]
>
> TypeScript consumers must use `"moduleResolution": "nodenext"/"node16"/"bundler"` in `tsconfig.json`.
> The legacy `"node"` resolver is not supported.

# Usage

| Module                 | Description                  |
|------------------------|------------------------------|
| [@metreeca/llms][llms] | AI tasks and shared services |

[llms]: https://metreeca.github.io/llms/modules/_metreeca_llms.html

# Support

- open an [issue](https://github.com/metreeca/llms/issues) to report a problem or to suggest a new feature
- start a [discussion](https://github.com/metreeca/llms/discussions) to ask a how-to question or to share an idea

# License

This project is licensed under the Apache 2.0 License –
see [LICENSE](https://github.com/metreeca/llms?tab=Apache-2.0-1-ov-file) file for details.
