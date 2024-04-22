## Kustomize

This is an example with overlays.

## Gotchas

1. You cannot have the `replaces` section in a `base` kustmize file, because it will change the template prematurely. (i.e. `base/deployment` template variables will be replaced with actual values before the `overlay` is triggered)
