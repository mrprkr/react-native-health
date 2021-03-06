Get the most recent blood alcohol content value.

On success, the callback function will be provided with a `blood alcohol content` object containing the blood alcohol content `value`, and the `startDate` and `endDate` of the blood alcohol content sample. *Note: startDate and endDate will be the same as blood alcohol content samples are saved at a specific point in time.*

```javascript
AppleHealthKit.getLatestBloodAlcoholContent(null, (err: string, results: Object) => {
    if (err) {
        console.log("error getting latest blood alcohol content: ", err);
        return;
    }
    console.log(results)
});
```

```javascript
{
	value: 0.001, // Percent
	startDate: '2016-07-08T12:00:00.000-0400',
	endDate: '2016-07-08T12:00:00.000-0400'
}
```
