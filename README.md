# Youtube Player

[[pub packages]](https://pub.dartlang.org/packages/youtube_player)

A flutter plugin to play Youtube Videos without API Key in ranges of Quality(240p,360p,480p,720p and 1080p).

![DEMO](demo.gif) 

## Usage

#### 1\. Depend

Add this to you package's `pubspec.yaml` file:

```yaml
dependencies:
  youtube_player: ^0.2.0
```

#### 2\. Install

Run command:

```bash
$ flutter packages get
```

#### 3\. Import

Import in Dart code:

```dart
import 'package:youtube_player/youtube_player.dart';
```

#### 4\. Using Youtube Player

```dart
///
/// LOW = 240p
/// MEDIUM = 360p
/// HIGH = 480p
/// HD = 720p
/// FHD = 1080p
///
YoutubePlayer(
          source: "6rwu29ZAbh8",
          quality: YoutubeQuality.HD,
),
```


## Example

[Example sources](https://github.com/sarbagyastha/youtube_player/tree/master/example)



***Credit***

This plugin is a fork of [video_player](https://github.com/flutter/plugins/tree/master/packages/video_player) which supports youtube playback.
The controls used in the plugin is derived from [chewie](https://github.com/brianegan/chewie).

Cheers to [@Flutter Team] and [@Brian Egan](https://github.com/brianegan) for developing such useful plugin and packages.


## License

```
Copyright 2019 Sarbagya Dhaubanjar

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```