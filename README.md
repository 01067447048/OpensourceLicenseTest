## 1. Project Gradle

    buildscript {
        dependencies {
            classpath 'com.google.android.gms:oss-licenses-plugin:0.10.4'
        }
    }


## 2. App Gradle
    
    id 'com.google.android.gms.oss-licenses-plugin'

    implementation 'com.google.android.gms:play-services-oss-licenses:17.0.0'


## 3. OssLicensesMenuActivity

    Intent(applicationContext, OssLicensesMenuActivity::class.java).also {
                OssLicensesMenuActivity.setActivityTitle("오픈소스 라이선스")
                startActivity(it)
            }