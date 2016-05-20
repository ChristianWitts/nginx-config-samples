# Mapped Dispatch

| File  | Purpose   |
| :---- | :-------: |
| conf.d/discovery-json | Contains the JSON response for the /discover end-point |
| conf.d/mapping.conf | Contains the nginx `map` directive for the header attribute and maps to `upstream` directive identifier |
| conf.d/upstream.conf | Contains the upstream servers available for a given service |
| sites-available/my-services | Contains the basic `/` route which will be auto-magically forwarded to the correct end-point mapping, and a `/discover` end-point to find out what is available |
