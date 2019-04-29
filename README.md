Unity.Profiler.Ext
====
Adds deep call-graph into Unity's profiler.

```cs
public void Update()
{
    Debug.Log("A");
    Bar(1, 2);
    Zoo();
    UnityEngine.Debug.Log("DEBUG");
}
```

__Without Unity.Profiler.Ext__<br>
![before](before_pfext.PNG)<br>
<br>
__After enabling Unity.Profiler.Ext__<br>
![after](after_pfext.PNG)<br>

Usage
----
* [다운로드](https://github.com/pjc0247/Unity.Profiler.Ext/releases) 페이지에서 다운받은 패키지를 추가합니다.
* Window/Profiler.Ext 버튼을 클릭하면 프로파일러가 표시됩니다.

![e](menuitem.png)


Limitations
----
* 에디터 실행만 지원
* `Update` 메소드만 지원
    * 코루틴 / 이벤트 핸들러등은 TODO
    * 코루틴 DONE (v.0.2.1)
