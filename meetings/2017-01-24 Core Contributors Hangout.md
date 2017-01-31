# 2017-01-24 Core Contributors Hangout

## Attendees

* Andrea Falcone ([@asfalcone](https://github.com/asfalcone))
* Michael Furtak ([@mfurtak](https://github.com/mfurtak))
* Maksym Grebenets ([@mgrebenets](https://github.com/mgrebenets))
* Olivier Halligon ([@AliSoftware](https://github.com/AliSoftware))
* Josh Holtz ([@joshdholtz](https://github.com/joshdholtz))
* Helmut Januschka ([@hjanuschka](https://github.com/hjanuschka))
* Felix Krause ([@krausefx](https://github.com/krausefx))
* Jerome Lacoste ([@lacostej](https://github.com/lacostej))
* David Ohayon ([@ohwutup](https://github.com/ohwutup))
* Mark Pirri ([@mpirri](https://github.com/mpirri))
* Danielle Tomlinson ([@DanToml](https://github.com/DanToml))
* Manuel Wallner ([@milch](https://github.com/milch))

## Agenda

* 10 min - Introductions (everyone)
* 5 min - Discuss Google/Firebase deal (we're still here and committed. thank people for their understanding and commitment)
* 10 min - Everyone talks about what they know about/work on
* 10 min - Discuss processes (when to merge vs approve PR) & vision (want fastlane to grow in the beta/deploy depth. encourage plugins for other needs)
* 10 min - Do we want to meet again/regularly? What times work for people? What else can we do to support core contributors? Plan to tweet about contributors
* 15 min - Q & A

## Areas of knowledge and interest

| Person   |        City       | Area of knowledge and interest |
|----------|-------------------|--------------------------------|
| Andrea   | Boston, MA        | screengrab, supply, sigh       |
| Mike     | Boston, MA        | Android, screengrab, fastlane, fastlane_core, command-line processing & Commander, iTunes Transporter, plugins |
| Mark     | Boston, MA        | iOS, scan, gym, spaceship, plugins |
| David    | Boston, MA        | iOS, packaged-fastlane, snapshot, gym |
| Felix    | San Francisco, CA | everything |
| Dan      | Berlin, Germany   | infrastructure, packaged-fastlane (CocoaPods mac app), weird Ruby things, architecture and performance |
| Helmut   | Vienna, Austria   | fixing bugs across all products, spaceship, first experience with Ruby, RSpec code coverage
| Jerome   | Paris, France     | sigh, deliver, spaceship. Wants to suppose own infrastructure, support all the platforms they use (unity3d). Wants to talk more about unity3d and Fabric. fastlane_core |
| Josh     | Chicago, IL       | fastlane implementation, user facing features, fastlane_core |
| Manu     | Vienna, Austria   | ios tools, code signing |
| Olivier  | Rennes, France    | gym and scan, ruby in general, ios, setting up fastlane for new people, getting people set up with their new PRs. |
| Maksym   | Sydney, Australia | iOS developer, code signing and resigning (sigh and resign), unit tests, commandline, open to learning |

## Ideas

* **Helmut** - Can we introduce a spaceship-like layer for Android & Google Play? Something that exposes all of the possibilities in a nice API...
    * We noted that _supply_ is built on top of a Ruby Gem provided by Google, but that the API of that is not always easy to use. _supply_ could also be extended to do more
* **Jerome/Olivier** - Is it possible to add features for platforms outside of mobile?
    * Generally speaking, this will not be a great fit with fastlane’s vision. If people want to expand the kinds of apps that fastlane can handle, these would be good to explore in separate projects first (possibly building on top of _fastlane_core_). If changes need to be made to _fastlane_ itself, we’d need to make sure that we don’t introduce too many specifics for platforms that are not a core focus.
* **Olivier/Dan** - From experience with CocoaPods, they suggest that we manage the fastlane changelog as a file inside the repository, as opposed to letting it be an artifact of the release process that its generated from Git. The benefits they mentioned included better searchability and discoverability.

## Actions

Future meetings: Let’s try scheduling something for once a month - attendance being optional
