# mySpot



    public void visitorButtonPressed(View view) {
        Intent intent = new Intent(this, LogInActivity.class);
        startActivity(intent);

    }
    



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
        android:text="@string/welcomeString"
        android:textColor="#000000"
        android:textSize="24sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.52"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.085" />

    <Button
        android:id="@+id/labelButton"
        android:layout_width="210dp"
        android:layout_height="76dp"
        android:onClick="labelButtonPressed"
        android:text="@string/labelString"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />


    <Button
        android:id="@+id/button"
        android:layout_width="210dp"
        android:layout_height="76dp"
        android:layout_marginBottom="4dp"
        android:onClick="visitorButtonPressed"
        android:text="@string/visitorString"
        app:layout_constraintBottom_toTopOf="@+id/labelButton"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.501"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.833" />

    <Button
        android:id="@+id/button2"
        android:layout_width="210dp"
        android:layout_height="78dp"
        android:layout_marginTop="4dp"
        android:text="@string/securityString"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.501"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/labelButton"
        app:layout_constraintVertical_bias="0.187" />

</androidx.constraintlayout.widget.ConstraintLayout>



