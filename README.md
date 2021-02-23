# CardViewStroke

- activity_main.xml
```xml
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <androidx.cardview.widget.CardView
        android:layout_width="300dp"
        android:layout_height="wrap_content"
        app:cardCornerRadius="10dp"
        app:cardElevation="30dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent">

        <FrameLayout
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:background="@drawable/card_edge_purple" />

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_margin="16dp"
            android:gravity="center"
            android:orientation="horizontal">

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="Bantu tanyakan ke toko mengenai stock" />
        </LinearLayout>
    </androidx.cardview.widget.CardView>

</androidx.constraintlayout.widget.ConstraintLayout>
```

- card_edge_purple.xml
```xml
<?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android">

    <solid android:color="@android:color/transparent" />

    <size android:width="10dp" />

    <stroke
        android:width="0.1dp"
        android:color="@color/purple_700" />

    <padding
        android:bottom="0dp"
        android:left="0dp"
        android:right="0dp"
        android:top="0dp" />

    <corners
        android:bottomLeftRadius="10dp"
        android:bottomRightRadius="10dp"
        android:topLeftRadius="10dp"
        android:topRightRadius="10dp" />

</shape>
```

![](https://github.com/gzeinnumer/CardViewStroke/blob/master/preview/example1.jpg)

---

```
Copyright 2021 M. Fadli Zein
```