
This is the Home Page for the community organization that maintain Viro, an open source developer platform for rapidly building AR/VR applications.

[Get started 🚀](https://github.com/ViroCommunity/starter-kit)

## Resources 📦

- [Chat](https://discord.gg/H3ksm5NhzT)
- [ViroReact Documentation](https://viro-community.readme.io/docs)
- [ViroCore Documentation](https://virocommunitycore.readme.io)

## GitHub Repos

- [Awesome Viro](https://github.com/ViroCommunity/awesome-viro)
- [Viro](https://github.com/ViroCommunity/viro)
- [Viro Core](https://github.com/ViroCommunity/virocore)
- [Viro Media App](https://github.com/ViroCommunity/viro-media-app)

## Maintainers Around The World 🤗

- [Adelar da Silva Queiróz](https://adelarsq.github.io) 🇧🇷
- [Eduardo Dorantes](https://github.com/doranteseduardo) 🇲🇽
- [George Ivanov](https://github.com/geo-vi) 🇦🇹 
- [Marian Šámal](https://github.com/mariansam) 🇨🇿
- [Paul McCabe](https://github.com/bilewinters) 🇬🇧
- [Robert Colley](https://github.com/robertjcolley) 🇺🇸


## Why Viro?

A great testimonial from Michael McClenaghan about Viro vs Unity ([source](https://discord.com/channels/774471080713781259/774471080713781263/789284272707338250)):

> "There are quite a few reasons we're trying to get away from Unity as a Library:

> 1. Iteration time. Getting your UaaL-enabled RN app built changes from taking a few minutes to upwards of 20-30 minutes or more when you factor in exporting the Xcode Project/Android Project from Unity and then building your wrapping framework. Any time you want to change something in the Unity AR, you have to re-export the Unity project, ensure that your integration into your RN xcworkspace wasn't broken in the process, and then build your RN app (which usually includes re-building all of the IL2CPP code, which is what adds ages to the final build). This makes getting anything done painfully slow.

> 2. Automated builds. UaaL doesn't support the CI/CD tool we use (Bitrise), which is a big thing for us. I'm sure you could get Unity building using the CLI on CircleCI or something similar, but for us that's something we're not in a position to invest in right now.

> 3. Bundle size. Unity massively bloats your application. Just adding an empty UaaL project to your app adds 20MB+. If you add Vuforia or anything else, and start to add other assets, your app can quickly become > 100MB. For some areas of the world, this is fine, but others where space is precious, this is a problem.

> 4. Communication between Unity and RN. To do any sort of communication between your RN app and your Unity library, you have to go through multiple bridges. You'll find yourself passing data from RN to native (Java and Swift/ObjC), then passing it from there to Unity with their native interfaces. This introduces a whole number of points of failure, that are very difficult to debug due to reason #1. We built a communication layer that uses JSON messages to talk between these, but it's horribly complex and specific to our usecase, that any developers who didn't specifically work with it are not familiar enough to contribute.

> 5. The bulk of our developers are RN devs, not Unity devs. Moving to Viro means our current development team will be much more comfortable making adjustments and changes to our AR experience.

> 6. License fees. We fall in the category of companies that are required to use a Unity Pro license. For me to have 3-4 licenses for our senior devs to have access to Unity, this adds hundreds of dollars per month of license fees for a feature that is a minor part of our application. You also have to commit to 12 months of Pro for each seat, which means you're committing to a lot of money up front for a tool that won't be used by a dev for most of the year. We also had a bunch of issues with getting Unity to properly unload when we send users back to RN. We eventually got it to a state where we could properly unload it on most devices, but we still had an issue where if you unloaded it and reloaded it a number of times without completely restarting the app, Unity got slower and slower, despite us unloading it properly. UaaL also appears to be another one of what I call Unity's "box checking" features, where someone in management was like "We need to be able to do this!" and a few engineers build a proof of concept, ship it and move on to the next thing. There hasn't really been any improvement or updates to the approach since it was originally announced."
