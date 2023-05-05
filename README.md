# generate-random-sentence

Generate Random Sentence is an NPM package designed to help developers generate random sentences using JavaScript. This package provides an easy-to-use API that allows you to generate sentences with customizable lengths and word choices.

## Features:

**Generate Random Sentences:** The primary feature of the package is to generate random sentences, allowing you to create fake text for testing or prototyping purposes.

**Customizable Sentence Length:** The package allows you to set a minimum and maximum length for the sentences you generate, so you can generate sentences of any length you need.

**Generate random sentences with Lorem Ipsum Text:** In addition to using custom word choices, you can also generate sentences using the famous Lorem Ipsum text, which can be useful for generating filler text for design mockups.

**Simple and easy to use:** The package is designed to be simple and easy to use, with a straightforward API that makes it easy to integrate into your projects.

## Install

```
$ npm install generate-random-sentence
```

## Usage

```javascript
const generateRandomSentence = require("./node_modules/generate-random-sentence");
```

Every sentence starts with an uppercase letter and ends with a period.

By default the range of `minWords = 15`, `maxWords = 20`

```javascript
const randomSentence = generateRandomSentence();
console.log(randomSentence);
// => Turpis, id diam. a diam a in augue. eu ante, ante volutpat pulvinar metus.
```

Set a `minimum` and `maximum` length for the sentences.

```javascript
let minWords = 5,
  maxWords = 10;
console.log(generateRandomSentence(minWords, maxWords));
// => Sapien bibendum, urna et nibh consectetur ullamcorper enim.
```

To specify the number of words in the sentence, set both `minimum` and `maximum` same.

```javascript
let minWords = 5,
  maxWords = minWords;
console.log(generateRandomSentence(minWords, maxWords));
// => Nisi risus. ex Pellentesque In.
```
