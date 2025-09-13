# Serverless-Predictive-Autoscaling

## Dataset Description

We use the [Azure Functions Access Dataset (2020)](https://azurepublicdatasettraces.blob.core.windows.net/azurepublicdatasetv2/azurefunctions_dataset2020/azurefunctions-accesses-2020.csv.bz2), which contains anonymized traces of blob accesses from Azure Functions.

**Schema**

| Field                      | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| `Timestamp`                 | Access time in milliseconds since 1970 (Unix epoch)                        |
| `AnonRegion`                | Unique id for the region                                                   |
| `AnonUserId`                | Unique id for the user                                                     |
| `AnonAppName`               | Unique id for the application                                              |
| `AnonFunctionInvocationId`  | Unique id for the function invocation                                      |
| `AnonBlobName`              | Unique id for the blob accessed                                            |
| `BlobType`                  | Type of the blob accessed                                                  |
| `AnonBlobETag`              | Version of the blob accessed                                               |
| `BlobBytes`                 | Number of bytes of the blob                                                |
| `Read`                      | Indicates if the access is a read operation (`true`/`false`)               |
| `Write`                     | Indicates if the access is a write operation (`true`/`false`)              |
