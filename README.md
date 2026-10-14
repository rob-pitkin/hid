This repository hosts the [WebHID Standard](https://hid.spec.whatwg.org/). It is one of [many web standards](https://spec.whatwg.org/) developed by the [WHATWG community](https://whatwg.org/).

## Code of conduct

We are committed to providing a friendly, safe, and welcoming environment for all. Please read and respect the [Code of Conduct](https://whatwg.org/code-of-conduct).

## Contribution opportunities

Folks notice minor and larger issues with the WebHID Standard all the time and we'd love your help fixing those. Pull requests for typographical and grammar errors are also most welcome.

Issues labeled ["good first issue"](https://github.com/whatwg/hid/labels/good%20first%20issue) are a good place to get a taste for editing the WebHID Standard. Note that we don't assign issues and there's no reason to ask for availability either, just provide a pull request.

If you are thinking of suggesting a new feature, read through the [FAQ](https://whatwg.org/faq) and [Working Mode](https://whatwg.org/working-mode) documents to get yourself familiarized with the process.

We'd be happy to help you with all of this [on Chat](https://whatwg.org/chat).

## Pull requests

In short, change `index.bs` and submit your patch, with a [good commit message](https://github.com/whatwg/meta/blob/main/COMMITTING.md).

Please add your name to the Acknowledgments section in your first pull request, even for trivial fixes. The names are sorted lexicographically.

To ensure your patch meets all the necessary requirements, please also see the [Contributor Guidelines](https://github.com/whatwg/meta/blob/main/CONTRIBUTING.md). Editors of the WebHID Standard are expected to follow the [Maintainer Guidelines](https://github.com/whatwg/meta/blob/main/MAINTAINERS.md).

## Tests

Tests are an essential part of the standardization process and will need to be created or adjusted as changes to the standard are made. Tests for the WebHID Standard can be found in the `hid/` directory of [`web-platform-tests/wpt`](https://github.com/web-platform-tests/wpt).

A dashboard showing the tests running against browser engines can be seen at [wpt.fyi/results/hid](https://wpt.fyi/results/hid).

## Building "locally"

For quick local iteration, run `make`; this will use a web service to build the standard, so that you don't have to install anything. See more in the [Contributor Guidelines](https://github.com/whatwg/meta/blob/main/CONTRIBUTING.md#building).

## Explainer

Details about the API including example usage code snippets and its motivation, privacy, and security considerations are described in [EXPLAINER.md](./EXPLAINER.md). Support for WebHID in extension service workers is described in [WEBHID_IN_EXTENSION_SERVICE_WORKERS_EXPLAINER.md](./WEBHID_IN_EXTENSION_SERVICE_WORKERS_EXPLAINER.md).

## Implementation Status

This API is implemented in [Blink](https://source.chromium.org/chromium/chromium/src/+/main:third_party/blink/renderer/modules/hid/). It is available in browsers based on Chromium 89 and later, such as Google Chrome and Microsoft Edge. Individual Chromium-based browsers may choose to enable or disable this API. Chromium-based Android browsers do not support this API because Android itself does not provide a direct API for accessing HID devices ([Chromium issue 964441](https://crbug.com/964441)). For the same reason this API is not available in Android WebView ([Chromium issue 1164125](https://crbug.com/1164125)).
