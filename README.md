⚠️ This Repository has been moved to the new Company repo 👉🏿[here](https://github.com/Swift-Simplified/ss-classes-structs-enums). 👈🏾

⚠️ Below is the original README File

![Swift](readme-images/swift-simplified-logo.png)

[SwiftSimplified.com](find-my-swift-version.md) | [Swift.org](https://docs.swift.org).

Simplifying the official [Swift Language Guide](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/thebasics/) into [The Swift Handbook 📖](https://www.swiftsimplified.com/the-swift-handbook). 😍

![instructor](readme-images/instructor-profile.png) [*with Matthew Harding*](https://www.udemy.com/user/iosbfree/)
# How To: 👈
# Choose Between Classes, Structs and Enums
in a Swift playground 🛝

[Download](https://github.com/MatthewpHarding/FREE-PLAYGROUND-classes-structs-enums/archive/refs/heads/main.zip) this Swift playground file to run the example given in [Xcode](https://developer.apple.com/xcode).

## This Playground Teaches 👨🏻‍🏫
When to make the choice to use either a class, struct or enum. 

Sometimes it's difficult to know when to use certain types. Enums, structs and classes are very different but also quite similar too.


This Swift playground is a workspace to test out some of the differences of these types. The online bonus video provides tips directly from an iOS proffessional - don't forget to watch it!

💡 Tip: As a general rule, enums represent state, structs represent data and classes manage the system.

The general code of the Swift playground looks something like this:

```Swift
// MARK: - 📦 Sourcecode
enum PlaybackState {
    case idle
    case paused
    case playing
    case finished
}

struct Episode {
    let title: String
    let duration: Double
}

struct Program {
    let title: String
    let episodes: [Episode]
}

class VideoPlayer {
    private(set) var currentProgram: Program?
    private(set) var currentEpisode: Episode?
    private(set) var currentPlaybackState: PlaybackState
    
    init() {
        currentProgram = nil
        currentEpisode = nil
        currentPlaybackState = .idle
    }
    
    func play(program: Program, episode: Episode) {
        currentProgram = program
        currentEpisode = episode
        currentPlaybackState = .playing
    }
    
    func pause() {
        guard let _ = currentEpisode else {
            return
        }
        currentPlaybackState = .paused
    }
    
    func resume() {
        guard let _ = currentEpisode else {
            return
        }
        currentPlaybackState = .playing
    }
}

let episodes = [Episode(title: "The One with the Pig", duration: 35.00 * 60.00), Episode(title: "The One with the Spaceship", duration: 20.00 * 60.00), Episode(title: "The One with the Grilled Cheese", duration: 25.00 * 60.00)]
let friends = Program(title: "F.r.i.e.n.d.s.", episodes: episodes)

let videoPlayer = VideoPlayer()
videoPlayer.play(program: friends, episode: friends.episodes[0])
print(videoPlayer.currentEpisode?.title ?? "")
// << 🔵 Run Point
```

## How To Download ⬇️
You can download this Swift playground by clicking the `Code` button at the top of this page. 

## How To Run The Playground 🏃🏾‍♂️
This repo stores a Swift playground file which are run and executed within [Xcode](https://developer.apple.com/xcode) *(the tool used by developers to build apps)* and you simply need to double click the file.

## Why Learn In A Swift Playground 🛝
Swift playgrounds allow for rapid developmemt and provide a very fast and fluid thought-to-code process. There is no time taken to compile, build or install an app to an iOS simulator. Instead, the compilation time is fast and results are viewed almost immediately. 

The term "playground" is a very fitting name for both the feature and the file extension itself. It may be safe to assume that this feature was designed for "playing around"... or "learning" as we like to call it. 😆

## How To Become A Swift Engineer
Most companies that offer iOS developer jobs simply need to maintain an existing Swift system that has previoiusly been put in place. Creating the architecture and thinking about performance can be difficult and may require some expert knowledge, but they are not the needs of most companies. In fact, if you are interested in maintaining an existing system then the technology industry will be a huge market place in which to advertise your skills. 

With the interest of both parties in mind *(the business and the employee)* having great Swift knowledge and being able to write safe code will be the biggest focus - *which is great news!* 😃🥳🎉 

This means, all you need to do is 👉 **[learn Swift!](https://www.swiftsimplified.com/the-swift-handbook)** 👈

## Why Learn Swift
To become an iOS developer with a great salary who can work anywhere in the world using only a laptop and an internet connection. 

By studying the language all of the other pieces of the puzzle will fall into place. With a clear grasp of the Swift programming language it will be much easier to apply for jobs and to pass each test they provide. The rest will be provided to you as you learn whats required within that role for that specific company. 

**Step 1**: Learn Swift

**Step 2**: Get A Job  - *learn how to make apps*

**Step 3**: 🕺🏼💃🪩

## Support The Worlds no.1 Company 
Wouldn't it make sense to write software for the worlds no.1 most prifitable company? I mean.. if you want to gain a good career and live a wealthy lifestyle. 🤷🏼‍♂️

We are tyring to consolidate more than a decades commercial experience combined with the official Swift documentation into short online courses *(created for fast learning)*, so that our students can live happier and wealthier lives - simply by learning 1 language! 😎

Why not think about becoming an iOS developer making apps for Apple software. 🤔💭

## Swift Simplified Services 🧑🏼‍🔧👨🏾‍🔧👩🏻‍🔧

- 👉 **[The Swift Handbook 📖](https://www.swiftsimplified.com/the-swift-handbook)** [Take a look](https://www.swiftsimplified.com/the-swift-handbook).

	The Swift Handbook is our main online course, simplifiying the [Official Swift Programming Language Guide](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/thebasics/) within a Swift playground. [Take a look](https://www.swiftsimplified.com/the-swift-handbook).

- 👉🏿 **[Official Swift Language Guide](https://github.com/MatthewpHarding/SWIFTDOCS-1-the-basics)** [Try it](https://github.com/MatthewpHarding/SWIFTDOCS-1-the-basics).
	
	We converted the [Official Swift Programming Language Guide](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/thebasics/) into Swift playgrounds to run all of the code examples in [Xcode](https://developer.apple.com/xcode/). [Try it](https://github.com/MatthewpHarding/SWIFTDOCS-1-the-basics).

- 👉🏾 **[Free Swift Playgrounds](https://www.swiftsimplified.com/swift-playgrounds)** [Try it](https://www.swiftsimplified.com/swift-playgrounds).

	Our website contains downloadable [GitHub repos](https://github.com/MatthewpHarding/FREE-PLAYGROUND-combine), which are great for learning Swift. [Try it](https://www.swiftsimplified.com/swift-playgrounds).

- 👉🏼 **[Swift Career Blog](https://www.swiftsimplified.com/swift-career-blog)** [Try it](https://www.swiftsimplified.com/swift-career-blog).

	Our website has a blog all about the tech industry and how to climb your career faster. [Try it](https://www.swiftsimplified.com/swift-career-blog).

## [Swift Simplified .com](https://www.swiftsimplified.com)
![Swift Simplified .com](readme-images/swift-simplified-logo-footer.png)

[Website](https://www.swiftsimplified.com) | [Career Blog](https://www.swiftsimplified.com/swift-career-blog) | [Free Playgrounds](https://www.swiftsimplified.com/swift-playgrounds) | [The Swift Handbook 📖](https://www.swiftsimplified.com/the-swift-handbook)

🛠 *..let's live a better life, by learning Swift* 🚀

```Swift
let myLife = [learning, coding, happiness] 
```
Welcome to our community of [Swift Simplified](https://www.swiftsimplified.com) students!
### 🧕🏻🙋🏽‍♂️👨🏿‍💼👩🏼‍💼👩🏻‍💻💁🏼‍♀️👨🏼‍💼🙋🏻‍♂️🙋🏻‍♀️👩🏼‍💻🙋🏿💁🏽‍♂️🙋🏽‍♀️🙋🏿‍♀️🧕🏾🙋🏼‍♂️
