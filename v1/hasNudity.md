# Nudity detection

## How it works
We use ML models to detect nudity and give a `true` or `false` result, but we also add some extra information as in the classification of the image (if it is porn).

## How to use
Well, its pretty simple, just POST the file [here](http://api.legion-surveillance.co.uk/v1/hasNudity) as `multipart/form-data` under the id of `file` (currently only JPG's are supported.. we plan to expand this soon.) and then you should get a result.

An example response will be
```JSON
{
    "classification": "Porn",
    "result": true,
    "code": 200
}
```
