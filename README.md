# Quiz Game (Flutter)

A small multiple-choice quiz app built with Flutter. The questions cover Flutter basics like widgets and state.

## Features

- Start screen with the quiz logo and a "Start Quiz" button
- Purple-to-orange gradient background shared across screens
- Question screen with the answer choices shuffled into a random order
- Custom rounded answer buttons
- Four questions stored in `lib/data/questions.dart`

## Status

This is a work in progress. Right now the app shows only the first question, and tapping an answer does not do anything yet. There is no scoring or results screen.

## Tech Stack

- Flutter (Material widgets)
- Dart SDK `^3.11.0`
- `flutter_lints` for static analysis

## Getting Started

Make sure Flutter is installed and `flutter doctor` reports no issues for the platform you want to run on.

```bash
git clone https://github.com/SummerPandey/Quiz-Game-Flutter.git
cd Quiz-Game-Flutter
flutter pub get
flutter run
```

To pick a specific device, list them with `flutter devices` and pass one with `-d`, for example `flutter run -d chrome`.

### Platforms

The project includes platform folders for Android, iOS, web, macOS, Windows, and Linux.

## Project Structure

```
lib/
  main.dart              App entry point
  quiz.dart              Root widget; switches between the start and question screens
  start_screen.dart      Start screen with logo and start button
  questions_screen.dart  Shows the current question and its answers
  answer_button.dart     Styled answer button widget
  data/questions.dart    Quiz questions and answer choices
  models/questions.dart  QuizQuestion model with answer shuffling
assets/images/           Quiz logo
test/                    Widget tests
```

The Dart package name is `adv_basics`, so imports use `package:adv_basics/...`.

Note: `test/widget_test.dart` is still the default Flutter counter test and does not match this app yet, so `flutter test` will fail until it is updated.
