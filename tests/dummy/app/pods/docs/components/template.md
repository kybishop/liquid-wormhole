If you'd rather send a component than use a block template, you can set the
`send` property to either a component name or helper:

<div class="example-button-container">
  <button {{action 'toggleHello'}} class="btn btn-primary btn-embossed">
    Press Me
  </button>
  {{#if showHello}}
    {{liquid-wormhole send="hello-component" class="hello-world notification top-right"}}
  {{/if}}
</div>

```
<button {{action 'toggleHello'}}>
  Press Me
</button>

{{#if showHello}}
  {{liquid-wormhole send="hello-component" class="hello-world"}}
{{/if}}
```
