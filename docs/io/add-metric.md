# Add Metrics to Emittes IO

## Purpose
This is used to add custom mertics to Emittes.

## Registering custom metric
```js
// to create a metric you can do the following:
io.metric.add({
    'classifier': "example-metric", // Classifier must be a unique value for this Project
    'displayname': "example metric", // Display Name can be anything, This is just what it shows on the Emitters Dashboard
    'description': "This is a example metric for Emittes IO" // A small decscription of what this metric is.
})
```

## Update metric (once)
To update the metric you can do the following, however this will only update the mertic once
```js
io.metric.update(example-metric, "15")
```

## Update metric on Interval
Want to update a mertic automatically using a value
```js
io.metric.intervalUpdate(examp, object, updaterate)
```
You do not need to provide the Updaterate, this will default to 5seconds
