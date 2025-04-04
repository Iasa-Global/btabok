---
title: "Sustainable Uptime Pattern"
keywords: 
sidebar: mydoc_sidebar
toc: true
permalink: sustainable_uptime_pattern.html
folder: patterns
summary: "The Ambassador pattern is a structural design pattern used primarily in distributed computing to offload common client-side network-related tasks."

---

# Sustainable Uptime Pattern (Green Orchestrator)

## Overview

The zero uptime pattern is a design solution in sustainability to turn off services, including all resource consumption, when they are not being used. 

## Intent

The primary intent of the Sustainable Uptime pattern is to utilize the lowest possible number of resources at all times. It includes movement and location awareness of services based on their current load. 

## Structure

1. **Green Orchestrator**: Capture and predict utilization within availablity requirements and instantiate, move and turn off containers and services based on utilization, sustainability configuration. 

## Responsibilities

- **Telemetry**: Capture usage and scale

## Implementation

Below are 

### Java Example

```java
// RemoteService interface public interface RemoteService {     String fetchData(); }  // RealRemoteService implementation public class RealRemoteService implements RemoteService {     @Override     public String fetchData() {         // Simulate network call         return "Data from remote service";     } }  // Ambassador class public class Ambassador implements RemoteService {     private final RemoteService remoteService;      public Ambassador(RemoteService remoteService) {         this.remoteService = remoteService;     }      @Override     public String fetchData() {         // Logging         System.out.println("Fetching data...");          // Retry logic         int retries = 3;         while (retries > 0) {             try {                 String data = remoteService.fetchData();                 // Log success                 System.out.println("Data fetched successfully: " + data);                 return data;             } catch (Exception e) {                 retries--;                 // Log failure                 System.err.println("Failed to fetch data, retries left: " + retries);                 if (retries == 0) {                     throw e;                 }             }         }         return null;     } }  // Client public class Client {     public static void main(String[] args) {         RemoteService service = new Ambassador(new RealRemoteService());         System.out.println(service.fetchData());     } }
```

### Python Example

```python
`import logging import time  class RemoteService:     def fetch_data(self):         raise NotImplementedError  class RealRemoteService(RemoteService):     def fetch_data(self):         # Simulate network call         return "Data from remote service"  class Ambassador(RemoteService):     def __init__(self, remote_service):         self.remote_service = remote_service      def fetch_data(self):         # Logging         logging.info("Fetching data...")          # Retry logic         retries = 3         while retries > 0:             try:                 data = self.remote_service.fetch_data()                 # Log success                 logging.info("Data fetched successfully: %s", data)                 return data             except Exception as e:                 retries -= 1                 # Log failure                 logging.error("Failed to fetch data, retries left: %d", retries)                 if retries == 0:                     raise e                 time.sleep(1)  # Backoff  if __name__ == "__main__":     logging.basicConfig(level=logging.INFO)     service = Ambassador(RealRemoteService())     print(service.fetch_data())`
```

### Mermaid Diagram

```mermaid
classDiagram     class Client {         +main(args: String[]): void     }      class RemoteService {         <>         +fetchData(): String     }      class RealRemoteService {         +fetchData(): String     }      class Ambassador {         -RemoteService remoteService         +fetchData(): String     }      Client --> Ambassador     Ambassador --> RemoteService     RealRemoteService --> RemoteService
```

#### Benefits

- **Separation of Concerns**: By isolating cross-cutting concerns, the pattern promotes cleaner and more maintainable code.
- **Reusability**: The Ambassador can be reused across different clients requiring the same remote service.
- **Resilience**: Implements retry and circuit breaking mechanisms, enhancing system robustness.

#### Use Cases

- **Microservices**: Ideal for managing interactions between microservices where network reliability and latency are concerns.
- **Third-party APIs**: Useful when interacting with third-party services to handle network-related complexities.

By implementing the Ambassador pattern, developers can significantly reduce the boilerplate code in clients and focus on core functionality, thus improving the overall architecture of distributed systems.

## Related Patterns

Scalability Patterns
