# Build
Execute `script.sh` to build the project. You will receive one file in the `dist` directory:
* **feed-webhook** is the app executable

# TODOs / Ideas
## Tests
Add more tests.
## Docs
Write docs and improve this README
## Formatters
Add functionality to allow to change what is sent to a webhook. JSONPath 
could be used to select values from the generated JSON and map them to 
a key. Example config:
```json
{
    "Formatters": [
        {
            "ID": "111-222-333-444",
            "Type": "jsonPath",
            "Output": {
                "Value1": "$.Title",
                "Value2": "$.Link.Href"
            }
        }
    ]
} 
```