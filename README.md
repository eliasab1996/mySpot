<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"

    android:background="@color/grey"
    android:orientation="vertical"
    tools:context=".ProfileFragment">

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
            android:text="Profile"
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
                            android:text="@string/UserString"
                            android:textSize="17sp"
                            android:textStyle="bold" />

                        <Space
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_weight="1" />

                        <ImageButton
                            android:id="@+id/refreshButton"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_gravity="center"
                            android:layout_marginStart="0dp"
                            android:layout_marginEnd="0dp"
                            android:background="@null"
                            android:src="@drawable/ic_refresh"
                            android:textSize="14sp" />

                        <Button
                            android:id="@+id/submitButton"
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginStart="0dp"
                            android:layout_marginEnd="0dp"
                            android:layout_weight="1"
                            android:background="@null"
                            android:text="Submit changes"
                            android:textColor="#FFCF66"
                            android:textSize="14sp" />
                    </LinearLayout>

                    <LinearLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content"
                        android:layout_marginTop="10dp"
                        android:orientation="vertical">

                        <LinearLayout
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:gravity="center_vertical"
                            android:paddingRight="8dp">

                            <ImageView
                                android:layout_width="40dp"
                                android:layout_height="40dp"
                                android:background="@drawable/circular_grey_bordersolid"
                                android:padding="10dp"
                                android:src="@drawable/ic_phone" />

                            <EditText
                                android:id="@+id/numOfUser"
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:layout_marginLeft="20dp"
                                android:background="@color/design_default_color_background"
                                android:hint="Write your phoneNo"
                                android:singleLine="false"
                                android:textColor="@color/goodgrey"
                                android:textSize="15sp"
                                android:visibility="visible" />
                        </LinearLayout>

                        <LinearLayout
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginTop="10dp"
                            android:gravity="center_vertical"
                            android:paddingRight="8dp">

                            <ImageView
                                android:layout_width="40dp"
                                android:layout_height="40dp"
                                android:background="@drawable/circular_grey_bordersolid"
                                android:padding="10dp"
                                android:src="@drawable/ic_email" />

                            <TextView
                                android:id="@+id/emailOfUser"
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:layout_marginLeft="20dp"
                                android:textColor="@color/goodgrey"
                                android:text="eliasab@gmail.com"
                                android:textSize="15sp"/>
                        </LinearLayout>

                        <LinearLayout
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginTop="10dp"
                            android:gravity="center_vertical"
                            android:paddingRight="8dp">

                            <ImageView
                                android:layout_width="40dp"
                                android:layout_height="40dp"
                                android:background="@drawable/circular_grey_bordersolid"
                                android:padding="10dp"
                                android:src="@drawable/ic_dorm" />

                            <Spinner
                                android:id="@+id/dorms"
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:layout_marginLeft="20dp"
                                android:text="East-Dorms"
                                android:textSize="15sp"
                                android:textColor="@color/goodgrey" />
                        </LinearLayout>

                        <LinearLayout
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginTop="10dp"
                            android:gravity="center_vertical"
                            android:paddingRight="8dp">

                            <ImageView
                                android:layout_width="40dp"
                                android:layout_height="40dp"
                                android:background="@drawable/circular_grey_bordersolid"
                                android:padding="10dp"
                                android:src="@drawable/ic_accessible" />

                            <Spinner
                                android:id="@+id/accOfUser"
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:layout_marginLeft="20dp"
                                android:text="No"
                                android:textSize="15sp"
                                android:textColor="@color/goodgrey" />
                        </LinearLayout>

                        <LinearLayout
                            android:layout_width="wrap_content"
                            android:layout_height="wrap_content"
                            android:layout_marginTop="10dp"
                            android:gravity="center_vertical"
                            android:paddingRight="8dp">

                            <ImageView
                                android:layout_width="40dp"
                                android:layout_height="40dp"
                                android:background="@drawable/circular_grey_bordersolid"
                                android:padding="10dp"
                                android:src="@drawable/ic_car" />


                            <Spinner
                                android:id="@+id/labelColors"
                                android:layout_width="wrap_content"
                                android:layout_height="wrap_content"
                                android:layout_marginLeft="20dp"
                                android:text="White-Blue"
                                android:textSize="15sp"
                                android:textColor="@color/goodgrey" />

                        </LinearLayout>


                    </LinearLayout>
                </LinearLayout>


            </LinearLayout>


        </LinearLayout>


    </ScrollView>

</RelativeLayout>
