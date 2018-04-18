+# 第二次实验
+## 1.实验目标
+(1)在Issues中创建自己的选题：https://github.com/hzuapps/android-labs-2018/issues； 
+(2)根据自选题目，编写一个或多个Activity（所有均带上学号前缀，放到自己的Java包下）； 
+(3)将标题设置为自己的学号+对应的功能或题目；
+## 2.实验步骤
+(1)阅读实验要求：https://github.com/hzuapps/android-labs-2018/labels/Lab 
+(2)在电脑上Android Studio编写代码 // 代码要可以运行！
+(3)使用Git将代码提交到自己的库中：https://github.com/Miles1212/android-labs-2018
+$ git pull 
+$ git add 学号目录/*
+$ git commit "#2 #992 第二次实验 "
+$ git push
+(4)在自己的GitHub库上创建和发送Pull Request（注意查看Changed files） // 是否只修改了自己的文件？ 
+(5)在GitHub中使用Markdown文件编写实验报告（report1.md, report2.md）// 保存在自己的文件夹下 
+## 3.实验结果(4个文件的代码)
+
+文件1.java\soft1614080902307\androidlabs\hzuapps\edu\soft1614080902307activity\Soft1614080902307Activity.java
+package soft1614080902307.androidlabs.hzuapps.edu.soft1614080902307activity;
+
+import android.os.Bundle;
+import android.support.design.widget.FloatingActionButton;
+import android.support.design.widget.Snackbar;
+import android.support.v7.app.AppCompatActivity;
+import android.support.v7.widget.Toolbar;
+import android.view.View;
+import android.view.Menu;
+import android.view.MenuItem;
+
+public class Soft1614080902307Activity extends AppCompatActivity {
+
+    @Override
+    protected void onCreate(Bundle savedInstanceState) {
+        super.onCreate(savedInstanceState);
+        setContentView(R.layout.activity_soft1614080902302);
+        Toolbar toolbar = (Toolbar) findViewById(R.id.toolbar);
+        setSupportActionBar(toolbar);
+
+        FloatingActionButton fab = (FloatingActionButton) findViewById(R.id.fab);
+        fab.setOnClickListener(new View.OnClickListener() {
+            @Override
+            public void onClick(View view) {
+                Snackbar.make(view, "Replace with your own action", Snackbar.LENGTH_LONG)
+                        .setAction("Action", null).show();
+            }
+        });
+    }
+
+    @Override
+    public boolean onCreateOptionsMenu(Menu menu) {
+        // Inflate the menu; this adds items to the action bar if it is present.
+        getMenuInflater().inflate(R.menu.menu_soft1614080902302, menu);
+        return true;
+    }
+
+    @Override
+    public boolean onOptionsItemSelected(MenuItem item) {
+        // Handle action bar item clicks here. The action bar will
+        // automatically handle clicks on the Home/Up button, so long
+        // as you specify a parent activity in AndroidManifest.xml.
+        int id = item.getItemId();
+
+        //noinspection SimplifiableIfStatement
+        if (id == R.id.action_settings) {
+            return true;
+        }
+
+        return super.onOptionsItemSelected(item);
+    }
+}
+
+文件2.AndroidManifest.xml
+
+<?xml version="1.0" encoding="utf-8"?>
+<manifest xmlns:android="http://schemas.android.com/apk/res/android"
+    package="soft1614080902307.androidlabs.hzuapps.edu.soft1614080902307activity">
+
+    <application
+        android:allowBackup="true"
+        android:icon="@mipmap/ic_launcher"
+        android:label="@string/app_name"
+        android:roundIcon="@mipmap/ic_launcher_round"
+        android:supportsRtl="true"
+        android:theme="@style/AppTheme">
+        <activity
+            android:name=".Soft1614080902302Activity"
+            android:label="@string/app_name"
+            android:theme="@style/AppTheme.NoActionBar">
+            <intent-filter>
+                <action android:name="android.intent.action.MAIN" />
+
+                <category android:name="android.intent.category.LAUNCHER" />
+            </intent-filter>
+        </activity>
+    </application>
+
+</manifest>
+
+文件3.activity_soft1614080902307.xml
+
+<?xml version="1.0" encoding="utf-8"?>
+<android.support.design.widget.CoordinatorLayout xmlns:android="http://schemas.android.com/apk/res/android"
+    xmlns:app="http://schemas.android.com/apk/res-auto"
+    xmlns:tools="http://schemas.android.com/tools"
+    android:layout_width="match_parent"
+    android:layout_height="match_parent"
+    tools:context=".Soft1614080902307Activity">
+
+    <android.support.design.widget.AppBarLayout
+        android:layout_width="match_parent"
+        android:layout_height="wrap_content"
+        android:theme="@style/AppTheme.AppBarOverlay">
+
+        <android.support.v7.widget.Toolbar
+            android:id="@+id/toolbar"
+            android:layout_width="match_parent"
+            android:layout_height="?attr/actionBarSize"
+            android:background="?attr/colorPrimary"
+            app:popupTheme="@style/AppTheme.PopupOverlay" />
+
+    </android.support.design.widget.AppBarLayout>
+
+    <include layout="@layout/content_soft1614080902307" />
+
+    <android.support.design.widget.FloatingActionButton
+        android:id="@+id/fab"
+        android:layout_width="wrap_content"
+        android:layout_height="wrap_content"
+        android:layout_gravity="bottom|end"
+        android:layout_margin="@dimen/fab_margin"
+        app:srcCompat="@android:drawable/ic_dialog_email" />
+
+</android.support.design.widget.CoordinatorLayout>
+
+文件4.strings.xml
+
+<resources>
+    <string name="app_name">Soft1614080902307数字小游戏</string>
+    <string name="action_settings">Settings</string>
+</resources>
+
+
+## 4.实验体会 
+ 通过本次实验,第一次创建android项目，并选择了自己的选题，完成了标题栏的更改。