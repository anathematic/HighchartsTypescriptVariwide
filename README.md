# Highcharts Variwide charts in Typescript

This project is a dummy project for an issue in Variwide charts + Typescript for Highcharts.

Bootstrapped with [Create React App](https://github.com/facebook/create-react-app), you can replicate at hand with:

```
yarn install
yarn start
```

And you should receive something along the lines of:

```
Type error: Type '{ type: "variwide"; }' is not assignable to type 'ChartOptions'.
  Types of property 'type' are incompatible.
    Type '"variwide"' is not assignable to type '"area" | "arearange" | "areaspline" | "areasplinerange" | "bar" | "boxplot" | "bubble" | "column" | "columnrange" | "errorbar" | "funnel" | "gauge" | "heatmap" | "line" | "pie" | ... 7 more ... | undefined'.  TS2322

     7 |
     8 | const options: Highcharts.Options = {
  >  9 |   chart: {
       |   ^
    10 |     type: 'variwide'
    11 |   },
    12 |
```

If there's a Highcharts-React exception, chances are `node_modules/@types/highcharts-react-official/index.d.ts` was removed and you will need to add it back.
