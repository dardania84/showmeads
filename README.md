# Description
![Alt Text](https://github.com/robinsalehjan/showmeads/blob/master/showmeads.gif)

## Folders
- Components: UI and XIB related files
- Controllers: Application logic
- Services: Abstraction for external services such as the JSON API and Core Data
- Utilities: Helper classes
- Extensions: Functions added as extensions to the `Foundation` classes

## Classes
- `AppDelegate`: Initalizes an `UINavigationController` with an instance of the `AdCollectionViewController` class as the root view controller
- `AdCollectionViewController`: The view controller manages and provides logic for the generic `UICollectionView` and the `AdCollectionViewCell`
- `AdsFacade`: A `Facade` abstraction with an simpler interface for the `AdService` and `AdPersistenceService` services
  - `AdService`: Responsible for fetching and parsing the response from the API to domain entities.
  - `AdPersistenceService`: Responsible for fetching, saving and deleting entities to and from Core Data

The `AdCollectionViewController` is the glue between the UI layer and the service layer. All requests made in the `AdCollectionViewController` instance to external services goes through the API provided by the `AdsFacade` class.

# Proud of
I managed to finish the project before my deadline (Wednesday).

# Could have been better
The UI does not have the the polish that I would like it to have. 
