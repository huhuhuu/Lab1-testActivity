# Lab1-testActivity
### description:
This is my first Android project, and I uploaded it to GitHub using git tools. 
This program demonstrates "Hello World" and validates the life cycle of Activity.
### core code:
```public class MainActivity extends AppCompatActivity {
    public static final String TAG = "MainActivity";
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Log.d(TAG,"onCreate");
    }
    @Override
    protected void onStart() {
        super.onStart();
        Log.d(TAG,"onStart");
    }
    @Override
    protected void onResume() {
        super.onResume();
        Log.d(TAG,"onResume");
    }
    @Override
    protected void onPause() {
        super.onPause();
        Log.d(TAG,"onPause");
    }
    @Override
    protected void onStop() {
        super.onStop();
        Log.d(TAG,"onStop");
    }
    @Override
    protected void onDestroy() {
        super.onDestroy();
        Log.d(TAG,"onDestroy");
    }
    @Override
    protected void onRestart() {
        super.onRestart();
        Log.d(TAG,"onRestart");
    }
}
```
### screenshots:
1.application start, execute onCreate(), onStart(), onResume().
![This picture is saved in the screenshot folder.](https://github.com/huhuhuu/Lab1-testActivity/blob/master/screenshot/first%20run%20application.PNG)
<br>2.click HOME button, execute onPause(), onStop().
![This picture is saved in the screenshot folder.](https://github.com/huhuhuu/Lab1-testActivity/blob/master/screenshot/after%20click%20HOME.PNG)
<br>3.return to the application, execute onRestart(), onStart(), onResume().
![This picture is saved in the screenshot folder.](https://github.com/huhuhuu/Lab1-testActivity/blob/master/screenshot/return%20to%20the%20application.PNG)
<br>4.click return button, execute onPause(), onStop(), onDestroy().
![This picture is saved in the screenshot folder.](https://github.com/huhuhuu/Lab1-testActivity/blob/master/screenshot/click%20return%20button%2Cthe%20application%20had%20been%20destory.PNG)
<br>5.this a picture of a Android program's live.
<br><img src="https://developer.android.google.cn/images/activity_lifecycle.png" align="left">
