# subtitle_wrapper_package

[![](https://img.shields.io/badge/pub-v1.0.2-brightgreen.svg)](https://pub.dev/packages/subtitle_wrapper_package)
[![flutter test automation](https://github.com/Joran-Dob/flutter_subtitle_wrapper/workflows/flutter%20test%20automation/badge.svg)](https://github.com/Joran-Dob/flutter_subtitle_wrapper/actions)
[![codecov](https://codecov.io/gh/Joran-Dob/flutter_subtitle_wrapper/branch/master/graph/badge.svg)](https://codecov.io/gh/Joran-Dob/flutter_subtitle_wrapper)

## Features

* Displaying of webvtt/srt subtitles 
* Loading of webvtt/srt subtitles from network
* Subtitle styling 

## Installation

This widget wraps the video player and displays the vtt subtitles on top. 

``` dart
@override
  Widget build(BuildContext context) {

    return Padding(
      padding: const EdgeInsets.all(12.0),
      child: Card(
          elevation: 2.0,
          child: SubTitleWrapper(
              videoPlayerController: videoPlayerController,
              subtitleController: SubtitleController(
                subtitleUrl: subtitleUrl,
                showSubtitles: true,
              ),
              subtitleStyle:
                  SubtitleStyle(textColor: Colors.white, hasBorder: true),
              videoChild: Chewie(
                controller: chewieController,
              ),
            ),
          ),
    );

  }

```

## Example

Demonstrates how to use the subtitle_wrapper_package plugin.

See the [example documentation](example/README.md) for more information.

## Changelog

See [CHANGELOG.md](CHANGELOG.md).

## Contributing

Feel free to contribute by opening issues and/or pull requests. Your feedback is very welcome!

## License

MIT License

Copyright (c) [2019] [Joran Dob]
