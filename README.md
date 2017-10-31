# ActiveAndroid-Sqlcipher

使用方法
１．将 ActiveAndroid　导入到项目依赖
２．将 assets jniLibs　放到项目app/src/main　下
３．在 mainfest.xml　里配置加密密码
	<meta-data
		    android:name="AA_DB_PWD"
		    android:value="alex"/>
或代码里面设置加密密码：
	Configuration configuration=new Configuration.Builder(this)
                .setDatabasePwd("password")
                .create();
        ActiveAndroid.initialize(configuration,true);

