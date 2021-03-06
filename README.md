[![Release](https://jitpack.io/v/abbas-oveissi/MaterialSearchView.svg)](https://jitpack.io/#abbas-oveissi/MaterialSearchView)

# MaterialSearchView
تنها تفاوت این کتابخانه با کتابخانه ی اصلی در این هست که همیشه بصورت راست به چپ نمایش داده می شود.حتی اگر در اندروید های 4.1 یا 4.0 از آن استفاده کنید.لینک کتابخانه ی اصلی در زیر قابل مشاهده هست :

<a href="https://github.com/MiguelCatalan/MaterialSearchView">https://github.com/MiguelCatalan/MaterialSearchView</a>

![sample](https://raw.githubusercontent.com/MiguelCatalan/MaterialSearchView/master/art/voice.gif) ![sample](https://raw.githubusercontent.com/MiguelCatalan/MaterialSearchView/master/art/default.gif)


#Native version
Maybe it would be useful to take a look into the new official approach

http://www.materialdoc.com/search-filter/

# Usage
نحوه ی استفاده از کتابخانه :

1- کد زیر را به فایل گردل اصلی پروژه اضافه کنید.
```javascript
	allprojects {
		repositories {
			...
			maven { url "https://jitpack.io" }
		}
	}
```
2- کد زیر را به فایل گردل ماژول خود اضافه کنید.
```javascript
	dependencies {
    	compile 'com.github.abbas-oveissi:materialsearchview:1.0.4'
	}
```
3-   در پایان برای نمایش ویو در اکتیویتی،کد زیر را در فایل ایکس ام ال آن قرار دهید.
```javascript
    <!-- Must be last for right layering display -->
    <FrameLayout
        android:id="@+id/toolbar_container"
        android:layout_width="match_parent"
        android:layout_height="wrap_content">

        <android.support.v7.widget.Toolbar
            android:id="@+id/toolbar"
            android:layout_width="match_parent"
            android:layout_height="?attr/actionBarSize"
            android:background="@color/theme_primary" />

        <ir.oveissi.materialsearchview.MaterialSearchView
            android:id="@+id/search_view"
            android:layout_width="match_parent"
            android:layout_height="wrap_content" />
    </FrameLayout>
```


# License
	Copyright 2015 Abbas Oveissi

	Licensed under the Apache License, Version 2.0 (the "License");
	you may not use this file except in compliance with the License.
	You may obtain a copy of the License at

		http://www.apache.org/licenses/LICENSE-2.0

	Unless required by applicable law or agreed to in writing, software
	distributed under the License is distributed on an "AS IS" BASIS,
	WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
	See the License for the specific language governing permissions and
	limitations under the License.
