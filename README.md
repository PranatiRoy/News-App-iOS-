![](https://raw.githubusercontent.com/TheCodeMonks/NYTimes-iOS/master/NYTimes%20Screenshots/Banner%400.25x.png)
![SwiftUI](https://img.shields.io/badge/Interface-SwfitUI-red)
![Architecture](https://img.shields.io/badge/Architecture-MVVM-green)




# NYTimes

New York Times is an Minimal News 🗞 iOS application built to describe the use of **SwiftSoup** and **CoreData** with **SwiftUI**.

## ⛓ Features

<table style="width:100%">
  <tr>
    <th>Articles Loading </th>
    <th>Browse by Category</th> 
  </tr>
  <tr>
    <td><img src="https://raw.githubusercontent.com/TheCodeMonks/NYTimes-iOS/master/NYTimes%20Screenshots/gifs/HomeLoading.gif" width=250 height=600 /></td> 
    <td><img src="https://raw.githubusercontent.com/TheCodeMonks/NYTimes-iOS/master/NYTimes%20Screenshots/gifs/browseByCategories.gif" width=250 height=600 /></td> 
  </tr>
  <tr>
    <th>Bookmark a Article using 3D Touch. </th>
    <th>Deleting bookmarks is just one swipe away</th> 
  </tr>
  <tr>
    <td><img src="https://raw.githubusercontent.com/TheCodeMonks/NYTimes-iOS/master/NYTimes%20Screenshots/gifs/bookmark3d.gif" width=250 height=600 /></td>
    <td><img src="https://github.com/TheCodeMonks/NYTimes-iOS/blob/master/NYTimes%20Screenshots/gifs/manageBookmark.gif" width=250 height=600 /></td>
  </tr>
</table>

## 📝 Table of Contents  
- [Requirements](#requirements)
- [Topic Focused](#topicfocused)
- [Technical Background](#techbackground)
- [Dependencies](#dependencies)
- [Project Structure](#projectstructure)





<a name="requirements"/>

## ⚙️ Requirements
```
iOS 14+
Xcode 12.2 and Up
```

<a name="topicfocused"/>

## 📚 Topic Focused
- Technologies
  - SwiftUI
  - CoreData
  - Combine
  - Web Scraping
- Design patterns from this project such as
  - Dependency injection
  - Repository 
  - Singleton
  - Observers
- MVVM Two way binding Architecture for SwiftUI with Combine framework is used.

<a name="techbackground"/>

## 🛠 Technical Background
- NYTimes App was made using SwiftUI as the Core interface with Two Way Binding MVVM Architecture using Combine framework. 
- CoreData is used to store the Article Bookmarks offline in device so that the user can access it at later time.
- SwiftSoup is used to scrap the required details from the NYTimes website.
- The User interface of this app mostly uses the inbuilt iOS components to keep the User experience close to the native feel.
- Bookmarks can be added as easy as a 3d-touch from Homescreen or a tap in bookmark icon in the detailed article screen.
- This project was built in the mindset of modularity and good coding patterns. Multiple design patterns like Dependency injection, Repository pattern, Singleton Pattern etc.

<a name="dependencies"/>

## 🔗 Dependencies

This project uses SPM (Swift Package Manager) as Dependency manager.

 - [SwiftSoup](https://github.com/scinfu/SwiftSoup)
 - [Kingfisher](https://github.com/onevcat/Kingfisher)
 - [Reachability](https://github.com/ashleymills/Reachability.swift)

<a name="projectstructure"/>

## ⛓ Project Structure

    NYTimes                 # Root Group
    .
    ├── Utilities           # Utilities for Fetching data ans Scraping HTML
    ├── Extensions          # Some useful extensions
    ├── Globals             # Contains App constants
    ├── Persistence         # Coredata files. Contains coredata model and Singleton for ManagedObjectContext
    ├── Views               # SwiftUI Views
    ├── Repository          # Repository for Coredata
    ├── ViewModel           # Viewmodels for SwiftUI Views
    ├── Model               # Model files
    |   └── Coredata Model  # Coredata model subclasses
    |
    └── Supporting files    # Misc. files like Appdelegate, SceneDelegate.

## Architecture
    
This app uses MVVM architecture.

![MVVM](https://raw.githubusercontent.com/TheCodeMonks/NYTimes-iOS/master/NYTimes%20Screenshots/MVVM.jpeg)



```
