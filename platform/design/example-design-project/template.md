# template

## Example Template

This template includes the following content types:

* Header
* Call-to-Action
* List of Documents needed

Below is a full example of the Example Template:

```text
---
title: Example Project
concurrence: complete
source: http:[ source info here ]
template: 4-action-page-pending
---

<div class="main" role="main" markdown="0">

<div class="va-action-bar--header">
  <div class="row">
    <div class="small-12 columns">
      <a class="usa-button-primary va-button-primary" href="[ Call-to-Action URL ]">[ Call-to-Action Copy ]</a>   // <---- This is Your Call-to-Action
    </div>
  </div>
</div>

<div class="section one" markdown="0">
<div class="primary" markdown="0">
<div class="row" markdown="0">
<div class="small-12 columns usa-content" markdown="1">
<div markdown="1">
[ Header Copy ] // <---- This is Your Header Copy
</div>
<div class="call-out usa-content" markdown="1">
### Which Documents will I need?   // <---- This is Sidebar Documents list
- [name of document](place document url here)
- [name of document](place document url here)
- [name of document](place document url here)

</div>
</div>

</div>
</div>
</div>

</div>
```

## Special Code Notes:

If you need to add a special class to the documents list, make sure it is done in the following way:

```text
- List item 1
- List item 2
- List item 3
{:.special-class-for-list}
```

Do you have a question about other classes or ids? Please refer to the [Markdown Style Guide](https://github.com/billfienberg/va.gov-team/tree/5839d463da035612a60148d7f90403dd12c8107e/platform/design/example-design-project/www.vets.gov)

