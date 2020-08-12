---
id: flyout
title: fast-flyout
sidebar_label: flyout
custom_edit_url: https://github.com/microsoft/fast/edit/master/packages/web-components/fast-foundation/src/flyout/README.md
---

An implementation of a [text field](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Input/text) as a form-connected web-component. The `fast-flyout` supports two visual appearances, outline and filled, with the control defaulting to the outline appearance.

## Usage

```html live
<fast-design-system-provider use-defaults>
    <fast-flyout >Flyout Content</fast-flyout>
</fast-design-system-provider>
```

## Applying custom styles

```ts
import { customElement } from "@microsoft/fast-element";
import { FlyoutTemplate as template, Flyout } from "@microsoft/fast-foundation";
import { FlyoutStyles as styles } from "./flyout.styles";

@customElement({
    name: "fast-flyout",
    template,
    styles,
})
export class FASTFlyout extends Flyout {}
```