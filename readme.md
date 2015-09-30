# Swift Workshop

## Outline
* Programming Languages
* iOS History
* Intro to Swift
* App demo and code tour
* Q/A
* Getting Set Up
* Going the distance

## Programming Languages

* [Part 1: Watch to 3:44](https://www.youtube.com/watch?v=vjtywpx2SDY&list=PL7141DE955793D3F0)
* [Part 3: Start at 3:44](https://youtu.be/rJelVDu3Aiw?list=PL7141DE955793D3F0&t=224)

I highly recomend watching the [rest of this series](https://www.youtube.com/playlist?list=PL7141DE955793D3F0) in your freetime.

## iOS History
* Objective-C
* Next
* Swift

## Intro to Swift

Swift is a modern, static typed, dynamic programming language used to write system and application code for OSX, iOS, and Watch-OS operating systems. Read the [brief intoduction by Apple](https://developer.apple.com/swift/) before moving on.

It's mostly what you know (loops, variables, functions, classes), but it has a number of unique features that make it stand out.

### Static Typing:
Swift is statically typed, which implies that you as the programmer must specify what type each variable is.

### Type inference
Type inference is when a programming language uses static typing, but can determine the type associated with a variable by its value when it is declared.

### Optionals
An optional value is one that might have a value or might not. That is to say, it will either be a value with the type specified, or nil. There are no other options. Here is an example use case:

```
func getHaterStatus(weather: String) -> String? {
    if weather == "sunny" {
        return nil
    } else {
        return "Hate"
    }
}
```

> Optionals remind me of checking for an error in JavaScript callbacks. They are not always going to be there, but you should always check for them. Similarly, Optionals don't walways have a nil value, but you should always check for one by unswrapping it.

### Arrays
```
var songs: [String] = ["Shake it Off", "You Belong with Me", "Back to December", 3]

var songs = [String]()



var songs = ["Shake it Off", "You Belong with Me", "Love Story"]
var songs2 = ["Today was a Fairytale", "White Horse", "Fifteen"]
var both = songs + songs2
```

### Dictionaries
```
var person = [
    "first": "Taylor",
    "middle": "Alison",
    "last": "Swift",
    "month": "December",
    "website": "taylorswift.com"
]

person["middle"]
person["month"]
```


```
var age = 25
"You are \(age) years old. In another \(age) years you will be \(age * 2)."
```


### Conditionals

```
var action: String
var person = "hater"

if person == "hater" {
    action = "hate"
} else if person == "player" {
    action = "play"
} else {
    action = "cruise"
}
```

```
if !stayOutTooLate && !nothingInBrain {
    action = "cruise"
}
```

### Loops
```
for i in 1...10 {
    print("\(i) x 10 is \(i * 10)")
}


var str = "Fakers gonna"

// Range
for _ in 1 ... 5 {
    str += " fake"
}

print(str)
```

### Looping over arrays

```
var people = ["players", "haters", "heart-breakers", "fakers"]
var actions = ["play", "hate", "break", "fake"]

for i in 0 ..< people.count {
    print("\(people[i]) gonna \(actions[i])")
}
```

### While loops
```
var counter = 0

while true {
    print("Counter is now \(counter)")
    ++counter

    if counter == 556 {
        break
    }
}
```

### Case

```
let studioAlbums = 5

switch studioAlbums {
case 0...1:
    print("You're just starting out")

case 2...3:
    print("You're a rising star")

case 4...5:
    print("You're world famous!")

default:
    print("Have you done something new?")
}
```

### Functions

```
func printAlbumRelease(name: String, year: Int) {
    print("\(name) was released in \(year)")
}

printAlbumRelease("Fearless", year: 2008)
printAlbumRelease("Speak Now", year: 2010)
printAlbumRelease("Red", year: 2012)
```

```
func albumsIsTaylor(name: String) -> Bool {
    if name == "Taylor Swift" { return true }
    if name == "Fearless" { return true }
    if name == "Speak Now" { return true }
    if name == "Red" { return true }
    if name == "1989" { return true }

    return false
}
```
### Optional types
```
func getName(status: String) -> String? {
    if status == "happy" {
      return "Aaron"
    } else {
      return nil
    }

}

getName("happy")
getName("Mad")
```

## App demo and code tour

## Q/A

## Getting Set Up
* Latest Xcode
* Shortcuts

## Going the distance
Work through [Hacking with Swift](https://www.hackingwithswift.com/read/0/overview/)

# Resources

## Reading
* [The Swift Programming Language, About Swift (iOS Developer Library)](https://developer.apple.com/library/prerelease/ios/documentation/Swift/Conceptual/Swift_Programming_Language/index.html#//apple_ref/doc/uid/TP40014097-CH3-XID_0)
* [Using Swift with Cocoa and Objective-C, Basic Setup (iOS Developer Library)](https://developer.apple.com/library/prerelease/ios/documentation/Swift/Conceptual/BuildingCocoaApps/index.html)
* [iOS Developer Library](https://developer.apple.com/library/ios/navigation/)
* [iOS Developer Library, Sample Code](https://developer.apple.com/library/prerelease/ios/navigation/#section=Resource Types&topic=Sample Code)
* [StackOverflow's Swift Info](http://stackoverflow.com/tags/swift/info)
* [StackOverflow's Swift Recent Questions](http://stackoverflow.com/questions/tagged/swift)
* [Unofficial Swift Online Compiler (Try Swift!)](http://swiftstub.com/)
* [iPhone Tutorials by Ray Wenderlich](http://www.raywenderlich.com/tutorials)
* [Hacking w/Swift eBook by Paul Hudson (free)](http://www.hackingwithswift.com/)

## Screencasts and Videos
* [unicorn.tv](https://swift.unicorn.tv/screencasts?page=2)
* [Swift Summit Conference Talks](https://realm.io/news/swift-summit/)
* [NSScreencasts](http://nsscreencast.com/episodes?page=10)

## Blogs
* [NSHipster](http://nshipster.com/)
* [CIMGF](http://www.cimgf.com/)
* http://jamesonquave.com/blog/developing-ios-apps-using-swift-tutorial/

## Courses
* [Stanford](https://itunes.com/StanfordSwift)
* https://www.youtube.com/playlist?list=PLC847C5B15C22BFDC
