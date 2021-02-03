# ReplayLatest

The ReplayLatest makes it simple for subscribers to share and receive the most recent values immediately upon subscription.

# Usage

Ensure to import ReplayLatest in each file you wish to have access to the utility.

The operators can then be used as part of your usual publisher chain declaration:

```swift
let subject = PassthroughSubject<Int, Never>()
let publisher = subject.replayLatest(capacity: 2)
```

# Debugging

ReplayLatest has a built-in printSink() operator that you can use to debug a subscription without the need to add a separate subscriber like so:

```swift
Just("value").printSink()
```

# Installation

Swift Package Manager:

```swift
dependencies: [
	.package(url: "https://github.com/abdalaliii/ReplayLatest.git")
]
```

# Developer Notes

This whole project is a work in progress, a learning exercise.


## License

**ReplayLatest** is available under the MIT license. See the LICENSE file for more info.
