## 🧠 Geo Hashing

The term “Geo-Hashing” refers to a method of encoding geographic coordinates (latitude & longitude) into a compact alphanumeric string. Nearby locations tend to share longer prefixes, making geohashes useful for spatial indexing and proximity queries in databases and real-time systems.
A spatial indexing and proximity search microservice built around geohashing techniques. This project encodes geographic coordinates into geohashes for efficient querying, location matching, and database spatial indexing. It demonstrates backend service patterns combined with frontend components for visualizing or interacting with geospatial data.

**Key features:**

* Convert latitude/longitude to geohashes
* Decode geohashes to geographic bounding boxes
* Support proximity searches for nearby drivers/locations
* gRPC and socket-based communication between components
  
---

### 🚗 1. Spatial Indexing for Rides/Drivers

Similar to how Uber historically used geospatial techniques (originally basic geohash and later the H3 system) to index driver & rider locations for efficient matching and dispatching. 

* A geohash implementation may help to quickly find nearby drivers based on passenger location.
* For example, if a rider’s geohash prefix matches a driver’s geohash, that driver is geographically close.

---

### 📌 2. Geohash Encoding/Decoding Library

The project might implement:

* Converting latitude/longitude into geohash codes.
* Decoding geohash back to coordinates or bounding boxes.
* Utility functions for proximity comparisons based on hash prefixes.

---

### 🛠 3. Integration with Networking / Backend


* Using **gRPC or socket connections** to transmit location updates.
* Backend microservices  handling geohash generation and queries.
* A frontend UI that optionally visualizes location data on a map or UI component.
