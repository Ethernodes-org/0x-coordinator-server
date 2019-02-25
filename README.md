## Table of contents

-   [Introduction](#introduction)
-   [Language choice](#language-choice)
-   [Getting started](#getting-started)
-   [Commands](#commands)
-   [Database](#database)
-   [Deployment](#deployment)
-   [Legal Disclaimer](#legal-disclaimer)

## Introduction

A reference server implementation of the TEC (TCC-flavor).

Fork this repository to get started!

## Getting started

#### Pre-requirements

-   [Node.js](https://nodejs.org/en/download/) > v8.x
-   [Yarn](https://yarnpkg.com/en/) > v1.x

To develop ontop of `0x-tec-server`, follow the following instructions:

1. Fork this repository

2. Clone your fork of this repository

3. Make sure you have [Yarn](https://yarnpkg.com/en/) installed.

4. Install the dependencies:

    ```sh
    yarn
    ```

5. Build the project

    ```sh
    yarn build
    ```

    or build & watch:

    ```sh
    yarn watch
    ```

6. Start the TEC server

    ```sh
    yarn start
    ```

## Commands

-   `yarn build` - Build the code
-   `yarn lint` - Lint the code
-   `yarn start` - Starts the relayer
-   `yarn watch` - Watch the source code and rebuild on change
-   `yarn prettier` - Auto-format the code

## Database

This project uses [TypeORM](https://github.com/typeorm/typeorm). It makes it easier for anyone to switch out the backing database used by this project. By default, this project uses an [SQLite](https://sqlite.org/docs.html) database.

## Deployment

`0x-tec-server` ships as a docker container. First, install Docker ([mac](https://docs.docker.com/docker-for-mac/install/), [windows](https://docs.docker.com/docker-for-windows/install/)). To build the image run:

```sh
docker build -t 0x-tec-server .
```

You can check that the image was built by running:

```sh
docker images
```

And launch it with

```sh
docker run -p 3000:3000 -d 0x-tec-server
```

## Legal Disclaimer

The laws and regulations applicable to the use and exchange of digital assets and blockchain-native tokens, including through any software developed using the licensed work created by ZeroEx Intl. as described here (the “Work”), vary by jurisdiction. As set forth in the Apache License, Version 2.0 applicable to the Work, developers are “solely responsible for determining the appropriateness of using or redistributing the Work,” which includes responsibility for ensuring compliance with any such applicable laws and regulations.
See the Apache License, Version 2.0 for the specific language governing all applicable permissions and limitations: http://www.apache.org/licenses/LICENSE-2.0
