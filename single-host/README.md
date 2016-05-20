# Single VHost routed dispatch

| File  | Purpose   |
| :---- | :-------: |
| conf.d/default.conf | Contains the server config which just includes the `services-available` for mappings |
| services.d/services-available/my-service{1,2} | Contains the `upstream` and `location` directives for a given service |
| services.d/services-available/discovery.conf | Contains the `/discover` end-point configuration |
