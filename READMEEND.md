## Explainer

Details about the API including example usage code snippets and its motivation, privacy, and security considerations are described in [EXPLAINER.md](./EXPLAINER.md). Support for WebHID in extension service workers is described in [WEBHID_IN_EXTENSION_SERVICE_WORKERS_EXPLAINER.md](./WEBHID_IN_EXTENSION_SERVICE_WORKERS_EXPLAINER.md).

## Implementation Status

This API is implemented in [Blink](https://source.chromium.org/chromium/chromium/src/+/main:third_party/blink/renderer/modules/hid/). It is available in browsers based on Chromium 89 and later, such as Google Chrome and Microsoft Edge. Individual Chromium-based browsers may choose to enable or disable this API. Chromium-based Android browsers do not support this API because Android itself does not provide a direct API for accessing HID devices ([Chromium issue 964441](https://crbug.com/964441)). For the same reason this API is not available in Android WebView ([Chromium issue 1164125](https://crbug.com/1164125)).
