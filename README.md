# BiliBili Stream Recorder

[![Build status](https://ci.appveyor.com/api/projects/status/1n4822yitgtu7ht7?svg=true)](https://ci.appveyor.com/project/Genteure/bililiverecorder)
[![Version](https://img.shields.io/github/tag/Bililive/BililiveRecorder.svg?label=Version)](#)
[![Issues are "help wanted"](https://img.shields.io/github/issues/Bililive/BililiveRecorder/help%20wanted.svg)](https://github.com/Bililive/BililiveRecorder/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
[![Pull Request Welcome](https://img.shields.io/badge/Pull%20request-welcome-brightgreen.svg)](#)
[![license](https://img.shields.io/github/license/Bililive/BililiveRecorder.svg)](#)

[简体中文 | Simplified Chinese](README_CN.md)

## Apology

GitHub is a global platform, and theoretically, everyone should use English. But since this project is only meant for Chinese user and rely on a Chinese website [BiliBili](https://live.bilibili.com) (_[wikipedia](https://en.wikipedia.org/wiki/Bilibili)_), all code comments are in Chinese. This README file will always use English so people like _you_ can understand what is this, and perhaps make some use out of it.

## Install & Use

See [rec.danmuji.org](https://rec.danmuji.org) (in Chinese)

## Feature

- Easy to use
- Reset timestamp to start from 0
- Writes duration info automatically when recoding session ends.
- Start recording when stream starts
- Record multiple stream at same time
- Pure C#, no native dependency like ffmpeg
- Open source!

## Develop & Getting Started

**Visual Studio 2017 with .NET Core** and **PowerShell** is required. Visual Studio 2019 *could* work but is not tested.

Some file are generated by [PreComplie Script](./CI/patch_buildinfo.ps1). Build project to clear errors shown by Visual Studio.

Project | Type | Note
:---:|:---:|:---
BililiveRecorder.WPF | .NET Framework 4.6.2
BililiveRecorder.Core | .NET Standard 2.0
BililiveRecorder.FlvProcessor | .NET Standard 2.0
BililiveRecorder.Server | .NET Core 2.0 | TODO

You can start poking around from...

- `BililiveRecorder.WPF/MainWindow.xaml` about WPF gui
- `BililiveRecorder.Core/Recorder.cs` about core record logic
- `BililiveRecorder.FlvProcessor/FlvStreamProcessor.cs` about FLV data process

## Reference & Acknowledgements

- [Adobe Flash Video File Format Specification 10.1.2.01.pdf](https://www.adobe.com/content/dam/acom/en/devnet/flv/video_file_format_spec_v10_1.pdf)
- [coreyauger/flv-streamer-2-file](https://github.com/coreyauger/flv-streamer-2-file)
- [zyzsdy/biliroku](https://github.com/zyzsdy/biliroku) - (probably) first BiliBili stream recording tool.
