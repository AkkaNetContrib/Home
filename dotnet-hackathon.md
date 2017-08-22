# .NET Foundation Summer Hackfest 2017

Welcome to the Summer Hackfest with Akka.NET!

[Akka.NET](http://getakka.net/) is a port of the JVM Akka distributed actor framework and it supports a large range of capabilities, runtimes, and plugins. Akka.NET is used in everything from Xamarin apps to WPF to large-scale distributed systems running on top of Windows Azure and Amazon.

## Goals for the Session
[We've recently released Akka.NET v1.3.0](https://github.com/akkadotnet/akka.net/releases/tag/v1.3.0), which added support for .NET Standard 1.6 to Akka.NET projects going forward. However, the vast majority of our plugins have not yet been ported to support .NET Standard, and thus that is the main focus of our participation in the .NET Foundation Summer Hackfest.

All of the plugins in the [Akka.NET Contrib organization](https://github.com/akkanetcontrib) need to be upgraded to support:

* MSBuild 15,
* .NET Standard 1.6 (not doing 2.0 yet due to its recency),
* .NET 4.5, for backwards compatibility with our current users for existing plugins, and
* Akka.NET 1.3.0.

## How to Contribute
First, start by taking a look at our [.NET Summer Hackfest milestone](https://github.com/AkkaNetContrib/Home/milestone/1). All of those issues are up for grabs and constitute projects that are designated as goals for the hackfest. 

Second, if you have some ideas for a new plugin that might be helpful to the Akka.NET community, [create an issue in this repository and submit it as part of the Hackfest](https://github.com/AkkaNetContrib/Home/issues/new?milestone=.NET+Summer+Hackfest). We can create a new repo inside this organization and help you setup CI and package publishing.

### Recommended Project Structure
Each project should have, at a minimum:

1. A `src/` folder with the root source code;
2. A readme that clearly explains what the project does, how to install it, and how to use it;
3. Unit tests to validate the integrity of the plugin; 
4. Apache 2.0 license; and
5. A build script capable of building, testing, and publishing each plugin to NuGet.

You can use the [`Petabridge.Templates`](https://github.com/petabridge/petabridge-dotnet-new) package with the `dotnet` CLI to scaffold a project with all of these requirements automatically. You can see an example [where a user did this with the Akka.TestKit.NUnit package here](https://github.com/AkkaNetContrib/Akka.TestKit.Nunit/pull/22).

## Communication
The Akka.NET core development team is here to help and you can [use our Gitter chat](https://gitter.im/akkadotnet/akka.net) to communicate with the team or you can post on any of the open issues in any repositories in this organization. We're here to help you setup CI, debug issues with the Akka.NET runtime, and get packages published to the [https://www.nuget.org/profiles/AkkaNetContrib](AkkaNetContrib NuGet account).

## Events
None as of yet, but we may schedule a virtual one later this week, but subscribe to [Gitter chat](https://gitter.im/akkadotnet/akka.net) to be notified.
