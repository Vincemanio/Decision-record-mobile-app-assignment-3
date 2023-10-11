# Data Storage 

## Status
Proposed

## Context
The creation of the retail company's new mobile app necessitates a number of data storage requirements in order to support features such as offline mode, push notifications, payment processing, user behavior tracking, and image storage. The need to determine the most efficient and scalable data storage solutions that cater to the specific needs of each feature while ensuring optimal app performance and responsiveness is driving this decision.

## Decision
We chose to  implement a local database system, such as SQLite, on the user's device for offline mode data storage. This local database will store critical data such as product information, order history, and other relevant content that users may require when they are not connected to the internet. The local database will act as a cache for critical data, allowing users to continue using the app's core features even when they have limited or no internet access. When an internet connection is established, the app will sync the local database with the server, updating it with any new data or changes made while the app was offline.

## Consequences
Users can continue to use the app's main features even when they are not connected to the internet, which improves the user experience. To ensure that data changes made offline are properly synced with the server once an internet connection is available, the app will need to implement a robust data synchronization mechanism. This approach simplifies offline access and ensures that users can interact with critical data even when they are not connected to the internet. To keep the local database up to date and in sync with the server, a well-designed data synchronization process is required.


Decision record template by Michael Nygard