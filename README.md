# lime-qml
[![Build Status](https://travis-ci.org/limetext/lime-qml.svg?branch=master)](https://travis-ci.org/limetext/lime-qml)
[![Coverage Status](https://img.shields.io/coveralls/limetext/lime-qml.svg?branch=master)](https://coveralls.io/r/limetext/lime-qml?branch=master)
[![Go Report Card](https://goreportcard.com/badge/github.com/limetext/lime-qml)](https://goreportcard.com/report/github.com/limetext/lime-qml)
[![GoDoc](https://godoc.org/github.com/limetext/lime-qml?status.svg)](https://godoc.org/github.com/limetext/lime-qml)

[![Bountysource Bounties](https://www.bountysource.com/badge/team?team_id=8742&style=bounties_received)](https://www.bountysource.com/teams/limetext/issues?utm_source=limetext&utm_medium=shield&utm_campaign=bounties_received)
[![Bountysource Raised](https://www.bountysource.com/badge/team?team_id=8742&style=raised)](https://www.bountysource.com/teams/limetext?utm_source=limetext&utm_medium=shield&utm_campaign=raised)

[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/limetext/lime)

This is the QML frontend for Lime. For more information about the project, please see [limetext/lime](https://github.com/limetext/lime).

## How to build
go: version 1.17.3

### Prerequisites

1. oniguruma

ubuntu 20 or above: 

```apt install libonig5```

ubuntu 18: 

Compile and install from source: https://github.com/kkos/oniguruma

2. Qt5Core Qt5Widgets Qt5Quick
```sh
sudo apt install libqt5quick5 qtdeclarative5-dev qtbase5-private-dev
```
### build 
```sh
go mod tidy
```
```sh
export CGO_CXXFLAGS="-I/usr/include/x86_64-linux-gnu/qt5/QtCore/5.9.5/"
make build
```