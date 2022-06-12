## 1. Research: Project Title 

- Keywords: 
  - flutter recognize text
  - Google_ml_kit
  - Flutter text recognition
  - flutter image recognition
  - flutter image text recognition
  - google ml kit text recognition flutter
- Video Title: Flutter Tutorial - Text Recognition - Using Google ML Kit [2022]


## 2. Research: Competitors

**Flutter Videos/Articles**

- https://aaqilsh.medium.com/how-to-use-google-ml-kit-package-in-flutter-for-text-recognition-206515b9c035
- https://pub.dev/packages/google_ml_kit
- 2.9K - https://www.youtube.com/watch?v=jZqTjFOxiC4
- 1.9K - https://www.youtube.com/watch?v=_sNOXGFJt8U
**Android/Swift/React Videos**

- 14K - https://www.youtube.com/watch?v=-7pM5ficYoc
- 4.8K - https://www.youtube.com/watch?v=9EKQ0UC04S8
- 2.1K - https://www.youtube.com/watch?v=N8JujDbUYmE
- 3.2K - https://www.youtube.com/watch?v=1ZbISHrgAnE

**Great Features** 
- NA

**Problems from Videos** 
- I want to read the text on the camera screen. E.g when the user click on the camera, text which  camera sees should be detected there, without capturing the image.
- Is it possible to extract the text as json?
- Bro does it detect any other language except english?
- How to extract arabic words , it deosn't work
- How to assign TextLines to different texteditingcontrollers.
For example i have three texteditingcontrollers - firsttext ,secondtext, thirdtext then how TextLines assign to different texteditingcontrollers in loop. Please describe in code.

for (TextBlock block in text.blocks) {
      for (TextLine line in block.lines) {
      }
    }

**Problems from Flutter Stackoverflow**

- https://stackoverflow.com/questions/66084486/using-google-ml-kit-on-device-text-recognition-in-flutter
- https://stackoverflow.com/questions/71658589/why-google-ml-kit-flutter-library-google-ml-kit-vision-took-large-size-while-t
## 3. Video Structure

**Main Points / Purpose Of Lesson**

1. Learn how to get text from image by using Google ML Kit Text Recognization
2. Learn how to use Clipboard in Flutter to Copy the text and using of showSnackBar [Note: Using '_key.currentState.ShowSnackBar(snackbar)' Is deprecated now.
This is the new way to add snackBars to the scaffold.
'ScaffoldMessenger.of(context).showSnackBar( SnackBar( content: Text("Incremented"), duration: Duration(milliseconds: 300), ), );']
3. Google's ML Kit for Flutter is a set of Flutter plugins that enable Flutter apps to use Google's standalone ML Kit. Google ML Kit have alot of Features, one of them is Text Regonisation and its the easiest way to get text from any image!

**The Structured Main Content**
1. First, Run this command with Flutter to add Google ML Kit in your pubspec.yaml [flutter pub add google_ml_kit]
2. To get photos from camera you must add camera to your AndroidManifest.xml in app/src/main/AndroidManifest.xml 
    - _[2. Pick Image From Gallery]_
    - _[3. Pick Image From Camera]_
3. you can get photos from your gallery or from your camera 
4. this loop to get all text from blocks and lines
for (TextBlock block in recognisedText.blocks) {
      for (TextLine line in block.lines) {
        scannedText = scannedText + line.text + "\n";
      }
    }
