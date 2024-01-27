# SwiftUI Siri Waveform

iOS9+ style customizable Siri waveform in SwiftUI

<img src="images/2019-09-14 23.05.03.gif" />

![alt text](https://i.ibb.co/QYNx40b/Screenshot-2023-11-25-at-13-09-45.png)

## Overview

This repo is a fork from [swiftui-siri-waveform-view](https://github.com/noahchalifour/swiftui-siri-waveform-view) repo which is now a public archive. This repo exposes the view as SPM Lib so it ca be easily integrated in modern SwiftUI projects.

This is a very simple implementation of the Siri waveform in iOS9+ made with SwiftUI. The math behind the waveform is based on a great article which [can be found here](https://www.freecodecamp.org/news/how-i-built-siriwavejs-library-maths-and-code-behind-6971497ae5c1/) that explains the math and builds a Siri waveform in Javascript.

## Installation

Swift Package Manager

File > Swift Packages > Add Package Dependency Add - Add https://github.com/nagu-code/SiriWaveView.git

## Usage

```swift
import SiriWaveView

struct MyView: View {

    @state var power: Double = 0.0

    var body: some View {
        VStack {
            SiriWaveView()
                .power(power)
        }
    }
}
```

Anytime the var power state is updated, the wave will animate automatically
