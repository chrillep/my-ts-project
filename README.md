# ʕ •́؈•̀) `workers-typescript-template`

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/8a2956a6646d4dae96df7de04fead0e4)](https://app.codacy.com/gh/chrillep/my-ts-project?utm_source=github.com&utm_medium=referral&utm_content=chrillep/my-ts-project&utm_campaign=Badge_Grade_Settings)
[![DeepSource](https://deepsource.io/gh/chrillep/my-ts-project.svg/?label=active+issues&show_trend=true&token=rb5EFUdloAKv57x9P0HENQ6b)](https://deepsource.io/gh/chrillep/my-ts-project/?ref=repository-badge)
[![Maintainability](https://api.codeclimate.com/v1/badges/be5255cf2225c094bd6f/maintainability)](https://codeclimate.com/github/chrillep/my-ts-project/maintainability)
[![Test Coverage](https://api.codeclimate.com/v1/badges/be5255cf2225c094bd6f/test_coverage)](https://codeclimate.com/github/chrillep/my-ts-project/test_coverage)
[![CodeFactor](https://www.codefactor.io/repository/github/chrillep/my-ts-project/badge)](https://www.codefactor.io/repository/github/chrillep/my-ts-project)
[![Total alerts](https://img.shields.io/lgtm/alerts/g/chrillep/my-ts-project.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/chrillep/my-ts-project/alerts/)
[![Language grade: JavaScript](https://img.shields.io/lgtm/grade/javascript/g/chrillep/my-ts-project.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/chrillep/my-ts-project/context:javascript)
[![codecov](https://codecov.io/gh/chrillep/my-ts-project/branch/master/graph/badge.svg?token=UxN04aS7tV)](https://codecov.io/gh/chrillep/my-ts-project)

A batteries included template for kick starting a TypeScript Cloudflare worker project.

## Note: You must use [wrangler](https://developers.cloudflare.com/workers/cli-wrangler/install-update) 1.17 or newer to use this template.

## 🔋 Getting Started

This template is meant to be used with [Wrangler](https://github.com/cloudflare/wrangler). If you are not already
familiar with the tool, we recommend that you install the tool and configure it to work with
your [Cloudflare account](https://dash.cloudflare.com). Documentation can be
found [here](https://developers.cloudflare.com/workers/tooling/wrangler/).

To generate using Wrangler, run this command:

```bash
wrangler generate my-ts-project https://github.com/cloudflare/worker-typescript-template
```

### 👩 💻 Developing

[`src/index.ts`](./src/index.ts) calls the request handler in [`src/handler.ts`](./src/handler.ts), and will return
the [request method](https://developer.mozilla.org/en-US/docs/Web/API/Request/method) for the given request.

### 🧪 Testing

This template comes with jest tests which simply test that the request handler can handle each request
method. `npm test` will run your tests.

### ✏️ Formatting

This template uses [`prettier`](https://prettier.io/) to format the project. To invoke, run `npm run format`.

### 👀 Previewing and Publishing

For information on how to preview and publish your worker, please see
the [Wrangler docs](https://developers.cloudflare.com/workers/tooling/wrangler/commands/#publish).

## 🤢 Issues

If you run into issues with this specific project, please feel free to file an
issue [here](https://github.com/cloudflare/workers-typescript-template/issues). If the problem is with Wrangler, please
file an issue [here](https://github.com/cloudflare/wrangler/issues).

## ⚠️ Caveats

The `service-worker-mock` used by the tests is not a perfect representation of the Cloudflare Workers runtime. It is a
general approximation. We recommend that you test end to end with `wrangler dev` in addition to
a [staging environment](https://developers.cloudflare.com/workers/tooling/wrangler/configuration/environments/) to test
things before deploying.
