# Storage service

Design
- [Azure Storage Scalability and Performance Targets](https://docs.microsoft.com/en-us/azure/storage/storage-scalability-targets)
- [Checklist](https://docs.microsoft.com/en-us/azure/storage/storage-performance-checklist)

Premium storage
- restricted to page blobs

Tools
- Storage Explorer

Naming conventions
- 3 up to 24 characters
- only lowercase letters and digits


Azure generates the following endpoints for access to four respective storage types:

- https://account_name.blob.core.windows.net/
- https://account_name.table.core.windows.net/
- https://account_name.queue.core.windows.net/
- https://account_name.file.core.windows.net/


## Monitoring

Aggregate metrics
- includes data such as the volume of ingress and egress traffic, availability, latency, or percentage of successful access requests aggregated for the Blob, Table, Queue, and File services.

Per-API metrics
- includes data representing volumes of storage API operations aggregated for the Blob, Table, Queue, and File services.

Logs
- These contain all storage operations for Blob, Table, Queue, and File services. This allows you to diagnose the cause of poor performance or to identify unauthorized access attempts.
