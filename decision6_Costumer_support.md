# Costumer support

## Status
Proposed

## context
The support for offline mode is a critical requirement in the development of the retail company's new mobile app. Customers can use this feature to browse products and view their order history even when they are not connected to the internet, with data syncing to the server once the connection is restored. The issue driving this decision is determining an appropriate data storage strategy that allows for seamless offline access while maintaining data integrity.

## Decision
We chose to implement a local database system, such as SQLite, on the user's device for offline mode data storage. This local database will store critical data such as product information, order history, and other relevant content that users may require when they are not connected to the internet. The local database will act as a cache for critical data, allowing users to continue using the app's core features even when they have limited or no internet access. When an internet connection is established, the app will sync the local database with the server, updating it with any new data or changes made while the app is offline.

## Consequences
this approach simplifies offline access and ensures that users can interact with critical data even when they are not connected to the internet. To keep the local database up to date and in sync with the server, a well-designed data synchronization process is required.

Decision record template by Michael Nygard