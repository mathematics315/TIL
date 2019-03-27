# 24時間以上をDateTimeとして使用したい場合

```csharp

var date = new DateTime(2012, 12, 15); // 12/15 00:00を作る
var span = new TimeSpan(25, 10, 0);    // 25時間10分　という時間間隔を作る
date = date.Add(span);                 // 12/15 00:00に時間間隔を加える

```
