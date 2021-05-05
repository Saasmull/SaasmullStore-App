# SaasmullStore

This is a Open-Source-AppStore from Saasmull where you can download free apps.

```java
    //define the path
    path = "storage/emulated/0/folder/app.apk";
    
    //check SDK for both installations
    if(android.os.Build.VERSION.SDK_INT < 26){
      //install for Android 7.1/SDK 25 and <
      StrictMode.setVmPolicy(new StrictMode.VmPolicy.Builder().build());
      Intent intent = new Intent(Intent.ACTION_VIEW);
      intent.setDataAndType(Uri.fromFile(new java.io.File(path)),"application/vnd.android.package-archive");
```
gjh
