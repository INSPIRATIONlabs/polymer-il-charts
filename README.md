polymer-il-charts
=================

This is a very flexible and customizable polymer charts library.

View [Component page](https://inspirationlabs.github.io/polymer-il-charts/components/polymer-il-charts/)

Currently supported chart types:

- Donut
- line charts
- multi line charts
- area charts
- stacked area charts
- spline charts
- spline area charts
- spline stacked area charts
- mixed area, line, spline, spline-area charts

## Example

Every color and every tooltip is configurable.

```js

<template id="auto-bind-date" is="auto-binding">
  <il-polymer-chart-donut data="{{data}}" width="{{width}}" height="{{height}}" cwidth="100" innermargin="100" datamargin="10">
  </il-polymer-chart-donut>
</template>
  <script>
    var t = document.querySelector('#auto-bind-date');
    var color = [
      '#00BCD4',
      '#26C6DA',
      '#4DD0E1',
      '#80DEEA',
      '#B2EBF2'
    ];
    t.width = 800;
    t.height = 800;
    t.data = {
       name: 'mytest',
       data: {
         test1: {
           values: [
             {value: 4.3},
             {value: 4.75, color: color[1] },
             {value: 2.75, color: color[2], tooltip: '<strong>test</strong>' },
             {value: 5, color: 'rgba(0,0,0,0)', tooltipdis: true},
             {value: 4.25, color: color[2] },
           ]
         },
         test2: {
           values: [
             {value: 2.35, color: color[4]},
             {value: 4.75, color: color[3]},
             {value: 4.86, color: color[2]},
             {value: 4.86, color: color[2]}
           ]
         },
         rund3: {
           values: [
             {value: 2.3, color: color[4]},
             {value: 2.3, color: color[3]},
             {value: 4.5, color: color[2]},
             {value: 2.3, color: color[3]},
           ]
         }
       }
     };
</script>
```

## Todo

- Add additional chart types
