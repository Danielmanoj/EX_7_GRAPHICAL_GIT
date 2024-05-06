# Ex_No-7_Graphical-Primitives
Design an application that draws basic graphical primitives on the screen.

## AIM:
To create and design an android application that draws basic graphical primitives on the screen using Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Min. required Artic Fox)


## ALGORITHM:

Step 1: Open Android Studio and then click on File -> New -> New project. </br>
Step 2: Then type the Application name as SMSIntent and click Next. </br>
Step 3: Select the Minimum SDK below and click Next. </br>
Step 4: Then select the Empty Activity and click Next. Finally, click Finish. </br>
Step 5: Design layout in activity_main.xml. </br>
Step 6: Draw the basic object processed in MainActivity file.</br>
Step 7: Save and run the application. </br>


## Program:

Program to create and design an android application for draw basic graphical primitives. </br>
Developed by: MANOJ G </br>
RegisterNumber:  212222240060 </br>


## MainActivity.java:
```
package com.example.exp7;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.graphics.Bitmap;
import android.graphics.Canvas;
import android.graphics.Color;
import android.graphics.Paint;
import android.graphics.drawable.BitmapDrawable;
import android.os.Bundle;
import android.widget.ImageView;
public class MainActivity extends AppCompatActivity {
```
```
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Bitmap bg = Bitmap.createBitmap(720, 1280,
                Bitmap.Config.ARGB_8888);
        ImageView i = (ImageView) findViewById(R.id.ImageView);
        i.setBackgroundDrawable(new BitmapDrawable(bg));
        Canvas canvas = new Canvas(bg);
        Paint paint = new Paint();
        paint.setColor(Color.RED);
        paint.setTextSize(50);
        canvas.drawText("Rectangle", 420, 150, paint);
        canvas.drawRect(400, 200, 650, 700, paint);
        canvas.drawText("Circle", 120, 150, paint);
        canvas.drawCircle(200, 350, 150, paint);
        canvas.drawText("Square", 120, 800, paint);
        canvas.drawRect(50, 850, 350, 1150, paint);
        canvas.drawText("Line", 480, 800, paint);
        canvas.drawLine(520, 850, 520, 1150, paint);

    }
}

```

## activity_main.xml:
```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout android:layout_height="match_parent"
    android:layout_width="match_parent"
    xmlns:android="http://schemas.android.com/apk/res/android">
    <ImageView
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:id="@+id/ImageView"/>
</RelativeLayout>
```

## Output: 
<img src="https://github.com/AmruthaRajsheker/EX_7_GRAPHICAL_GIT/assets/119475943/500c4541-c95a-4004-b603-c4271c402e43" alt="description" style="width: 40%; height: auto;">

## Result:
Thus a Simple Android Application to create and design an android application that draws basic graphical primitives on the screen using Android Studio was developed and executed successfully.
