# Coder Swag

[![Swift 5.0](https://img.shields.io/badge/Swift-5.0-orange?style=flat-square)](https://img.shields.io/badge/Swift-5.0-orange?style=flat-square)
[![iOS 16.0+](https://img.shields.io/badge/iOS-16.0%2B-blue?style=flat-square)](https://img.shields.io/badge/iOS-16.0%2B-blue?style=flat-square)
[![UIKit](https://img.shields.io/badge/UIKit-storyboards-lightgrey?style=flat-square)](https://img.shields.io/badge/UIKit-storyboards-lightgrey?style=flat-square)

A UIKit storyboard sample that opens on a Shop By Category screen for coder swag (hats, hoodies, shirts, digital).

## Overview

Coder Swag loads `Main.storyboard` from the classic `AppDelegate` lifecycle. The initial controller is a navigation stack with an orange bar and a white title, Coder Swag. Its root is `ViewController`. Below the bar, a label reads Shop By Category, and a plain table fills the safe area underneath. That table is connected to the `categoryTable` outlet.

The only prototype cell is `CategoryCell`, with a row height of 159. `categoryImage` is an image view pinned to the cell edges; the storyboard sets it to the `digital` asset. `categoryTitle` is a centered label over the image; the storyboard text is HOODIES. `ViewController` does not assign a data source or delegate, and `CategoryCell` does not set those outlets in code.

## Features

- A `UINavigationController` is the initial view controller, with `ViewController` as its root.
- A Shop By Category label sits above the table.
- The table is wired to the `categoryTable` outlet.
- The prototype cell is `CategoryCell`, with `categoryImage` and `categoryTitle` outlets.
- The asset catalog contains category images (`hats`, `hoodies`, `shirts`, `digital`) and product images (`hat01`–`hat04`, `hoodie01`–`hoodie04`, `shirt01`–`shirt05`).

## Requirements

| | |
| --- | --- |
| Xcode | 16 or later |
| iOS | 16 or later |
| Swift | 5 |

## Getting Started

```sh
git clone https://github.com/halilozel1903/CoderSwagApp.git
cd CoderSwagApp
open CoderSwagApp.xcodeproj
```

Choose an iOS 16+ simulator and run.

## Project structure

```text
.
├── README.md
├── CoderSwagApp.xcodeproj
│   ├── project.pbxproj
│   └── project.xcworkspace
│       ├── contents.xcworkspacedata
│       └── xcshareddata
│           └── IDEWorkspaceChecks.plist
└── CoderSwagApp
    ├── AppDelegate.swift
    ├── Info.plist
    ├── Controller
    │   └── ViewController.swift
    ├── View
    │   └── CategoryCell.swift
    ├── Base.lproj
    │   ├── LaunchScreen.storyboard
    │   └── Main.storyboard
    └── Assets.xcassets
        ├── Contents.json
        ├── AppIcon.appiconset
        │   └── Contents.json
        ├── digital.imageset
        │   ├── Contents.json
        │   └── digital.png
        ├── hats.imageset
        │   ├── Contents.json
        │   └── hats.png
        ├── hoodies.imageset
        │   ├── Contents.json
        │   └── hoodies.png
        ├── shirts.imageset
        │   ├── Contents.json
        │   └── shirts.png
        ├── hat01.imageset
        │   ├── Contents.json
        │   └── hat01.jpg
        ├── hat02.imageset
        │   ├── Contents.json
        │   └── hat02.jpg
        ├── hat03.imageset
        │   ├── Contents.json
        │   └── hat03.jpg
        ├── hat04.imageset
        │   ├── Contents.json
        │   └── hat04.jpg
        ├── hoodie01.imageset
        │   ├── Contents.json
        │   └── hoodie01.jpg
        ├── hoodie02.imageset
        │   ├── Contents.json
        │   └── hoodie02.jpg
        ├── hoodie03.imageset
        │   ├── Contents.json
        │   └── hoodie03.jpg
        ├── hoodie04.imageset
        │   ├── Contents.json
        │   └── hoodie04.jpg
        ├── shirt01.imageset
        │   ├── Contents.json
        │   └── shirt01.jpg
        ├── shirt02.imageset
        │   ├── Contents.json
        │   └── shirt02.jpg
        ├── shirt03.imageset
        │   ├── Contents.json
        │   └── shirt03.jpg
        ├── shirt04.imageset
        │   ├── Contents.json
        │   └── shirt04.jpg
        └── shirt05.imageset
            ├── Contents.json
            └── shirt05.jpg
```

## Current limitations

- `ViewController` does not implement a table data source or delegate, so the table does not show the category catalog.
- There is no product flow.
- `AppIcon.appiconset` has slots but no image files.

## Author

[Halil Özel](https://github.com/halilozel1903)
