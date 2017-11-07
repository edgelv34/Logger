# Logger
##### Logger 사용법은 간단합니다.
<pre>
<code>

Logger.d(" Message ");

</code>
</pre>

단지 사용할 때 Debug 인지 아닌지를 static 으로 선언해주시면 됩니다.

<pre>
<code>

public class AppConfig {

	private static boolean isDebuggable;

	public setDebuggable(boolean debug) {
		isDebuggable = debug;
	}

	public static boolean isDebuggable() {
		return isDebuggable;
	}

}

</code>
</pre>

#### getCallerInfo 메소드는 해당 클래스의 이름과 Logger 를 호출한 메소드의 이름을 나타냅니다.