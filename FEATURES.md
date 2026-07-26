<?xml version="1.0" encoding="utf-8"?>
<ScrollView xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@color/background"
    android:fillViewport="true">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        android:padding="32dp"
        android:gravity="center">

        <!-- Logo/Icon -->
        <ImageView
            android:layout_width="100dp"
            android:layout_height="100dp"
            android:src="@android:drawable/ic_lock_lock"
            android:tint="@color/primary"
            android:layout_marginBottom="20dp"/>

        <!-- App Title -->
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="PassShield"
            android:textSize="36sp"
            android:textStyle="bold"
            android:textColor="@color/primary"
            android:letterSpacing="0.05"
            android:layout_marginBottom="8dp"/>

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Secure Password Manager"
            android:textSize="14sp"
            android:textColor="@color/text_secondary"
            android:layout_marginBottom="40dp"/>

        <!-- Login Card -->
        <androidx.cardview.widget.CardView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            app:cardCornerRadius="16dp"
            app:cardElevation="4dp"
            android:layout_marginBottom="24dp">

            <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:orientation="vertical"
                android:padding="24dp">

                <TextView
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:text="Login"
                    android:textSize="20sp"
                    android:textStyle="bold"
                    android:textColor="@color/text_primary"
                    android:layout_marginBottom="20dp"/>

                <com.google.android.material.textfield.TextInputLayout
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:hint="Username"
                    style="@style/Widget.MaterialComponents.TextInputLayout.OutlinedBox"
                    app:boxStrokeColor="@color/primary"
                    android:layout_marginBottom="16dp">

                    <com.google.android.material.textfield.TextInputEditText
                        android:id="@+id/usernameInput"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:inputType="text"/>
                </com.google.android.material.textfield.TextInputLayout>

                <com.google.android.material.textfield.TextInputLayout
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:hint="Password"
                    style="@style/Widget.MaterialComponents.TextInputLayout.OutlinedBox"
                    app:boxStrokeColor="@color/primary"
                    app:endIconMode="password_toggle"
                    android:layout_marginBottom="20dp">

                    <com.google.android.material.textfield.TextInputEditText
                        android:id="@+id/passwordInput"
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:inputType="textPassword"/>
                </com.google.android.material.textfield.TextInputLayout>

                <Button
                    android:id="@+id/loginBtn"
                    android:layout_width="match_parent"
                    android:layout_height="56dp"
                    android:text="Login"
                    android:textSize="16sp"
                    android:textAllCaps="false"
                    android:backgroundTint="@color/primary"
                    android:textColor="@android:color/white"
                    app:cornerRadius="12dp"/>
            </LinearLayout>
        </androidx.cardview.widget.CardView>

        <!-- Biometric Login -->
        <androidx.cardview.widget.CardView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            app:cardCornerRadius="16dp"
            app:cardElevation="4dp">

            <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:orientation="vertical"
                android:padding="20dp"
                android:gravity="center">

                <TextView
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:text="or"
                    android:textSize="14sp"
                    android:textColor="@color/text_secondary"
                    android:layout_marginBottom="12dp"/>

                <Button
                    android:id="@+id/biometricLoginBtn"
                    android:layout_width="match_parent"
                    android:layout_height="56dp"
                    android:text="🔐 Biometric Login"
                    android:textSize="16sp"
                    android:textAllCaps="false"
                    style="@style/Widget.MaterialComponents.Button.OutlinedButton"
                    app:strokeColor="@color/primary"
                    app:cornerRadius="12dp"/>
            </LinearLayout>
        </androidx.cardview.widget.CardView>

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Your passwords are encrypted and secure"
            android:textSize="12sp"
            android:textColor="@color/text_secondary"
            android:layout_marginTop="24dp"
            android:gravity="center"/>

    </LinearLayout>
</ScrollView>
