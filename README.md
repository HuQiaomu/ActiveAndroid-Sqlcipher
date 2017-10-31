# ActiveAndroid-Sqlcipher
<br>
使用方法<br>
１．将 ActiveAndroid　导入到项目依赖 <br>
２．将 assets jniLibs　放到项目app/src/main　下　<br>
３．在 mainfest.xml　里配置加密密码<br>
```
	<meta-data
		    android:name="AA_DB_PWD"
		    android:value="alex"/>
```
或代码里面设置加密密码：<br>
```
	Configuration configuration=new Configuration.Builder(this)
                .setDatabasePwd("password")
                .create();
        ActiveAndroid.initialize(configuration,true);
```
