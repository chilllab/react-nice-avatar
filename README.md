# react-nice-avatar

[![Version](http://img.shields.io/npm/v/react-nice-avatar.svg)](https://www.npmjs.org/package/react-nice-avatar)
[![npm download][download-image]][download-url]

[download-image]: https://img.shields.io/npm/dm/react-nice-avatar.svg?style=flat-square
[download-url]: https://npmjs.org/package/react-nice-avatar

<div align="center">
    <a href="https://nice-avatar.chilllab.io/">
        <img src="https://user-images.githubusercontent.com/5305874/120076504-68e15980-c0d8-11eb-896c-3824b5eb05bb.png" 
             width="600" alt="imagewall" />
    </a>
</div>

## Online editor / preview

- https://nice-avatar.chilllab.io/

## Assets

- Designer: [@Micah](https://www.figma.com/@Micah) on Figma
- Figma files: [Avatar Illustration System](https://www.figma.com/community/file/829741575478342595)

## Installation

```sh
npm install react-nice-avatar
```

or

```sh
yarn add react-nice-avatar
```

## Usage

1. Import the component
    ```js
    import Avatar, { genConfig } from 'react-nice-avatar'
    ```
2. Generate random config, the config can be saved into your database to use later
    ```js
    const config = genConfig(AvatarConfig?)
    ```
3. Render the component with specific width / height and configuration
    ```jsx
    <Avatar style={{ width: '8rem', height: '8rem' }} {...config} />
    ```
    or
    ```jsx
    <Avatar className="w-32 h-32" {...config} />
    ```

## Options

The options can be passed into genConfig or as React props

|key|type|default|accept|tips
|---|---|---|---|---|
|id|string| | | Only for React Props
|className|string| | | Only for React Props
|style|object| | | Only for React Props
|shape|string|circle|circle, rounded, square| Only for React Props
|sex| string | | man, woman
|faceColor| string |
|earSize| string | | small, big
|hairColor| string |
|hairStyle| string | | normal, thick, mohawk, womanLong, womanShort
|eyeStyle| string | | circle, oval, smile
|glassesStyle| string | | none, round, square | Usually is none
|noseStyle| string | | short, long, round
|mouthStyle| string | | laugh, smile, peace
|shirtStyle| string | | hoody, short, polo
|shirtColor| string |
|bgColor| string |

## Development

1. Clone the repo:
    ```sh
    $ git clone git@github.com:chilllab/react-nice-avatar.git
    $ cd react-nice-avatar
    ```
2. Install dependencies:
    ```sh
    $ yarn
    ```
    Or
    ```sh
    $ npm install
    ```
3. Start the server for the demo:
    ```sh
    $ make dev
    ```
5. Open the browser to reivew the demo:
    ```sh
    $ open http://localhost:5555
    ```
7. Edit the files inside [src](/src).

## License

Released under [MIT](/LICENSE) by [@chilllab](https://github.com/chilllab).
