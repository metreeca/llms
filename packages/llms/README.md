# @metreeca/llms

[![npm](https://img.shields.io/npm/v/@metreeca/llms)](https://www.npmjs.com/package/@metreeca/llms)

AI tasks and shared services for [@metreeca/llms](https://github.com/metreeca/llms).

A job names the models it relies on by their contract rather than importing a concrete client. The
[@metreeca/gear](https://github.com/metreeca/gear) executor binds each contract to the implementation chosen for the
run.

Binding a different implementation leaves the job unchanged: the same job runs against a live provider, against
recorded responses, or against any custom client honouring the same contracts.

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
