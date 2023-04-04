# Day12_slider_button_flutter

This package provides an easy implementation of a Slider Button to cancel current transaction or screen. Highly customizable iphone alike looking widget

# 1-Add the  slider_button dependency in your pubspec.yaml file.

```
dependencies:
  slider_button: ^2.0.0
```

# 2-Import the  slider_button package in your dart file.

```
import 'package:slider_button/slider_button.dart';
```

# 3-use him like this

```
Center(child: SliderButton(
      action: () {
        ///Do something here
        Navigator.of(context).pop();
      },
       label: Text(
          "Slide to cancel Event",
          style: TextStyle(
              color: Color(0xff4a4a4a), fontWeight: FontWeight.w500, fontSize: 17),
        ),
      icon: Text(
        "x",
        style: TextStyle(
          color: Colors.white,
          fontWeight: FontWeight.w400,
          fontSize: 44,
        ),
      ),


    ));
```
