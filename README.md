# Avatar-glow

A new Flutter project.

## Getting Started

![avatar-glow](https://user-images.githubusercontent.com/86792533/183258672-db290aa1-64ae-4b94-b6bb-770c0145973e.png)



# Code 
#

```
import 'package:flutter/material.dart';
import 'package:avatar_glow/avatar_glow.dart';

class MyHomePage extends StatelessWidget {
  const MyHomePage({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Avatar-Glow'),

      ),
      body: Center(
        child: AvatarGlow(
          glowColor: Colors.red,
          endRadius: 90.0,
          duration: Duration(milliseconds: 2000),
          repeat: true,
          showTwoGlows: true,
          repeatPauseDuration: Duration(milliseconds: 100),
          child: Material(     // Replace this child with your own
            elevation: 8.0,
            shape: CircleBorder(),
            child: CircleAvatar(
              backgroundColor: Colors.grey[100],
              child: Icon(Icons.add),
              radius: 40.0,
            ),
          ),
        ),
      ),
    );
  }
}
```
