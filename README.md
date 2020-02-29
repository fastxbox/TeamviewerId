#Android get teamviewer id from log

Add it in your root build.gradle at the end of repositories:
在项目(app)的 build.gradle添加

```
	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```

Step 2. Add the dependency
```
	dependencies {
	        implementation 'com.github.fastxbox:TeamviewerId:1.0.0'
	}
```


使用方法
```
       String teamViewerId = TeamViewerHelper.getTeamviewerIDFromContent(this);
```
