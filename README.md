# Google DeepMind Gemini

Google Gemini is a set of cutting-edge large language models (LLMs) designed to be the driving force behind Google's future AI initiatives.

<img  alt="Gemini " src="https://raw.githubusercontent.com/ged-flod/google_gemini/main/assets/gemini.jpeg"/>

This package provides a powerful bridge between your Flutter application and Google's revolutionary Gemini AI. It empowers you to seamlessly integrate Gemini's capabilities into your app, unlocking a world of possibilities for building innovative, intelligent, and engaging experiences that redefine user interaction.



## Features

- [Set up your API key](#getting-started)
- [Initialize gemini](#initialize-gemini)
- [Content based APIs](#content-based-apis)
    - [Text-only input](#text-only-input)
    - [Text-and-image input](#text-and-image-input)
- [Gemini Candidates](#gemini-response)
- [Gemini Methods](#gemini-methods)



## Getting started

To use the Gemini API, you'll need an API key. If you don't already have one, create a key in Google AI Studio. [Get an API key](https://ai.google.dev/).

## Initialize gemini

To initialize gemini you must add init factory in main function.
```dart
void main() {

  /// add this line
  Gemini.init(apiKey: '--- Your Gemini Api Key ---');

  runApp(const MyApp());
}
```

Now you can create a instance

```dart
final gemini = Gemini.instance;
```

## Content based APIs

### Text-only input

This feature lets you perform natural language processing (NLP) tasks such as text completion and summarization.

```dart
  gemini.textInput("Write a story about a magic backpack.")
    .then((value) => print(value?.content?.parts?.last.text))
    .catchError((e) => print(e));
```

### Text-and-image input

If the input contains both text and image, You can send a text prompt with an image to the gemini-pro-vision model to perform a vision related task. For example, captioning an image or identifying what's in an image.

```dart
// In progress
```


## Gemini Response

```dart
// In progress
```

## Gemini Methods

```dart
// In progress
```