A feature is a method that can be applied to an object and will provide some kind of generic functionality.

All features should conform to the following interface:

```js
const ExampleFeature = function(config, host) {
    return ExampleFeatureInterface || undefined;
}
```

1. a feature is always a function
2. the name of the feature is always written in pascal-case and ends with the word `Feature`
3. a feature usually takes two arguments, first a configuration value and second the object that hosts the feature. If no configuration value is needed, the only argument is the host.
4. if a feature doesn't require a host argument, it's not a feature
5. a feature can either return an object that implements its interface or `undefined`