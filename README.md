# lifecycle
```
package com.example.myapplication;

import androidx.appcompat.app.AppCompatActivity;

import android.content.Intent;
import android.os.Bundle;
import android.view.View;
import android.widget.Toast;

public class PersonalActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_personal_activitity);
        Toast.makeText(this, "onCreate", Toast.LENGTH_SHORT).show();
    }
    protected void onStop(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_personal_activitity);
        Toast.makeText(this, "onStop", Toast.LENGTH_SHORT).show();
    }
    protected void onPause(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_personal_activitity);
        Toast.makeText(this, "onPause", Toast.LENGTH_SHORT).show();
    }
    protected void onResume(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_personal_activitity);
        Toast.makeText(this, "onResume", Toast.LENGTH_SHORT).show();
    }
    public void NextPage(View view){
        Intent i = new Intent(getApplicationContext(), SecondaryActivity.class);
        startActivity(i);
    }
}
```


```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Whatsapp!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView2"
        android:layout_width="120dp"
        android:layout_height="18dp"
        android:text="Click the button"
        tools:layout_editor_absoluteX="160dp"
        tools:layout_editor_absoluteY="420dp" />

    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Start Chat"
        tools:layout_editor_absoluteX="140dp"
        tools:layout_editor_absoluteY="494dp" />


</androidx.constraintlayout.widget.ConstraintLayout>
```
