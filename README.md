<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"

    android:background="@color/grey"
    android:orientation="vertical"
    tools:context=".HomeFragment">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="240dp"
        android:background="@color/blue" />

    <!--Top Header Layout-->
    <LinearLayout
        android:id="@+id/topbar"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_alignParentTop="true"
        android:gravity="center_vertical"
        android:padding="16dp">


        <Space
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1" />

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/HomeString"
            android:textColor="@color/white"
            android:textSize="20sp"
            android:textStyle="bold" />

        <Space
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1" />

    </LinearLayout>

    <ScrollView
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:scrollbars="none"
        android:layout_below="@+id/topbar">

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:orientation="vertical"
            android:paddingLeft="20dp"
            android:paddingTop="10dp"
            android:paddingRight="20dp">

            <!--Top Profile Section -->
            <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:background="@drawable/circularbordersolid"
                android:gravity="center"
                android:orientation="vertical"
                android:padding="16dp">

                <androidx.cardview.widget.CardView
                    android:layout_width="110dp"
                    android:layout_height="100dp"
                    app:cardCornerRadius="6dp"
                    app:cardElevation="0dp">

                    <ImageView
                        android:layout_width="110dp"
                        android:layout_height="100dp"
                        android:scaleType="centerCrop"

                        android:background="@drawable/ic_photo2"/>

                </androidx.cardview.widget.CardView>

                <LinearLayout
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:orientation="vertical">
                    <TextView
                        android:id="@+id/nameOfUser"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:layout_marginTop="10dp"
                        android:text="Elias Abo Sinni"
                        android:textColor="#424242"
                        android:textSize="21sp"
                        android:textStyle="bold" />

                </LinearLayout>


            </LinearLayout>

            <!--Option Bar-->

            <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginTop="10dp"
                android:layout_marginBottom="10dp"
                android:background="@drawable/circularbordersolid"
                android:gravity="center"
                android:orientation="horizontal">

                <TextView
                    android:id="@+id/welcome"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_weight="2"
                    android:gravity="center"
                    android:padding="13dp"
                    android:text="@string/welcomeString"
                    android:textAllCaps="true"
                    android:textColor="@color/blue"
                    android:textSize="14sp"
                    android:textStyle="bold" />

            </LinearLayout>

            <!--Bootom Cards with sections-->
            <LinearLayout
                android:id="@+id/personalinfo"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:orientation="vertical">



                <!--Contact Details-->
                <LinearLayout
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_marginTop="10dp"
                    android:background="@drawable/circularbordersolid"
                    android:orientation="vertical"
                    android:padding="16dp">

                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content">

                        <TextView
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:text="Services"
                            android:textSize="17sp"
                            android:textStyle="bold" />

                        <Space
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_weight="1" />


                    </LinearLayout>

                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="146dp"
                        android:layout_marginTop="10dp"
                        android:orientation="vertical">

                        <LinearLayout
                            android:layout_width="match_parent"
                            android:layout_height="match_parent"
                            android:gravity="center_vertical"
                            android:paddingRight="8dp">

                            <Space
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:layout_weight="1" />
                            <LinearLayout
                                    android:layout_width="wrap_content"
                                    android:layout_height="match_parent"
                                     android:orientation="vertical"
                                    >

                                <ImageView
                                    android:id="@+id/parkingIm"
                                    android:layout_width="90dp"
                                    android:layout_height="90dp"
                                    android:background="@drawable/circular_grey_bordersolid"
                                    android:padding="10dp"
                                    android:src="@drawable/ic_parking1" />

                                <TextView
                                    android:id="@+id/findSpot"
                                    android:layout_width="match_parent"
                                    android:layout_height="wrap_content"
                                    android:text="@string/findSpotStr"
                                    android:textSize="17sp"
                                    android:textStyle="bold"
                                    android:paddingLeft="10dp"
                                    android:paddingRight="10dp"
                                    android:lines="@integer/google_play_services_version"

                                    />
                            </LinearLayout>
                            <Space
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:layout_weight="1" />
                            <LinearLayout
                                    android:layout_width="wrap_content"
                                    android:layout_height="match_parent"
                                    android:orientation="vertical"
                                    >
                                <ImageView
                                    android:layout_width="90dp"
                                    android:layout_height="90dp"
                                    android:background="@drawable/circular_grey_bordersolid"
                                    android:padding="10dp"
                                    android:src="@drawable/ic_information1" />
                                <TextView
                                    android:id="@+id/parksInformation"
                                    android:layout_width="match_parent"
                                    android:layout_height="wrap_content"
                                    android:text="@string/parkingInformationStr"
                                    android:textSize="17sp"
                                    android:textStyle="bold"
                                    android:paddingLeft="10dp"
                                    android:paddingRight="10dp"
                                    android:lines="@integer/google_play_services_version"
                                    />
                            </LinearLayout>
                            <Space
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:layout_weight="1" />
                            <LinearLayout
                                    android:layout_width="wrap_content"
                                    android:layout_height="match_parent"
                                    android:orientation="vertical"     >                               >
                                <ImageView
                                    android:layout_width="90dp"
                                    android:layout_height="90dp"
                                    android:background="@drawable/circular_grey_bordersolid"
                                    android:padding="10dp"
                                    android:src="@drawable/ic_plan1" />
                                <TextView
                                    android:id="@+id/planMyDay"
                                    android:layout_width="match_parent"
                                    android:layout_height="wrap_content"
                                    android:text="@string/planMyDayStr"
                                    android:textSize="17sp"
                                    android:textStyle="bold"
                                    android:paddingLeft="10dp"
                                    android:paddingRight="10dp"
                                    android:lines="@integer/google_play_services_version"

                                    />
                            </LinearLayout>
                            <Space
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:layout_weight="1" />

                        </LinearLayout>

                        <LinearLayout
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:gravity="center_vertical"
                            android:paddingRight="8dp">


                        </LinearLayout>

                        <LinearLayout
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginTop="10dp"
                            android:gravity="center_vertical"
                            android:paddingRight="8dp">

                        </LinearLayout>

                        <LinearLayout
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginTop="10dp"
                            android:gravity="center_vertical"
                            android:paddingRight="8dp" />


                    </LinearLayout>
                </LinearLayout>


            </LinearLayout>


        </LinearLayout>


    </ScrollView>

</RelativeLayout>
