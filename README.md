<h1 align="center">Coder Swag</h1>

<p align="center">
  <a href="https://swift.org"><img alt="Swift 6.0" src="https://img.shields.io/badge/Swift-6.0-orange?style=flat"></a>
  <a href="https://developer.apple.com/ios/"><img alt="iOS 16.0+" src="https://img.shields.io/badge/iOS-16.0%2B-blue?style=flat"></a>
  <a href="https://developer.apple.com/documentation/uikit"><img alt="UIKit" src="https://img.shields.io/badge/UIKit-native-lightgrey?style=flat"></a>
</p>

<p align="center">A UIKit storyboard sample that opens on a Shop By Category screen for coder swag (hats, hoodies, shirts, digital).</p>

## Overview

Coder Swag is a UIKit storyboard sample for looking through coder swag by category: hats, hoodies, shirts, and digital items.

The first screen is a navigation stack. An orange navigation bar is titled Coder Swag. Under it, a Shop By Category label sits above a full-width table. Each row is a tall image cell.

## Features

- Orange navigation bar titled Coder Swag
- Shop By Category label
- Full-width table
- Tall image cells with a centered title

## Requirements

| Requirement | Version |
| --- | --- |
| Xcode | 16 or later |
| iOS | 16 or later |
| Swift | 6.0 |

## Getting Started

```sh
git clone https://github.com/halilozel1903/CoderSwagApp.git
cd CoderSwagApp
open CoderSwagApp.xcodeproj
```

Select the CoderSwagApp scheme, an iOS 16+ simulator, and run.

## Project structure

```text
.
├── CoderSwagApp.xcodeproj
└── CoderSwagApp
    ├── AppDelegate.swift
    ├── Info.plist
    ├── Controller
    │   └── ViewController.swift
    ├── View
    │   └── CategoryCell.swift
    ├── Base.lproj
    │   ├── Main.storyboard
    │   └── LaunchScreen.storyboard
    └── Assets.xcassets
```

The catalog holds category images `hats`, `hoodies`, `shirts`, and `digital`, and product images `hat01`–`hat04`, `hoodie01`–`hoodie04`, and `shirt01`–`shirt05`.

## Current limitations

- `ViewController` does not implement a table data source or delegate, so categories are not shown.
- There is no product flow.
- App icon slots have no image files.

## Author

[Halil Özel](https://github.com/halilozel1903)
