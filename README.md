# PopMenu


[![License](https://img.shields.io/github/license/imtianx/PopMenu.svg)](https://github.com/imtianx/PopMenu/blob/master/LICENSE) 
[![Stars](https://img.shields.io/github/stars/imtianx/PopMenu.svg)](https://github.com/imtianx/PopMenu/stargazers) 
[![Stars](https://img.shields.io/github/forks/imtianx/PopMenu.svg)](https://github.com/imtianx/PopMenu/network) 
[![Forks](https://img.shields.io/github/issues/imtianx/PopMenu.svg)](https://github.com/imtianx/PopMenu/issues) 

自定义对话框的使用，仿照ios。从底部弹出，类似pop窗口。包括消息、图片、列表及对话框。

演示效果：
![image](https://github.com/txadf/PopMenu/blob/master/1.gif)


使用方法：<br>
```
1,Add it in your root build.gradle at the end of repositories:
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
	    }
}
2,Add the dependency:
dependencies {
	        implementation 'com.github.OOOOOldZhu:PopMenu:1.2'
}
details please look the MainActivity.java	
new ActionSheetDialog(context).show();
new ActionSheetDialog(context).show();
```

注：context = 当前activity.this;

具体用法：
```
//(1)
new ActionSheetDialog (context)
   .builder()
   .setTitle ("清空消息列表后，聊天记录依然保留，确定要清空消息列表？")
   .setCancelable (false)
   .setCanceledOnTouchOutside (false)
   .addSheetItem ("清空消息列表", ActionSheetDialog.SheetItemColor.Red, new ActionSheetDialog.OnSheetItemClickListener(){
       @Override
       public void onClick (int which){

       }
   })
   .show();

//(2)
new ActionSheetDialog (context)
    .builder()
    .setTitle ("清空消息列表后，聊天记录依然保留，确定要清空消息列表？")
    .setCancelable (false)
    .setCanceledOnTouchOutside (false)
    .addSheetItem ("清空消息列表", ActionSheetDialog.SheetItemColor.Red, new ActionSheetDialog.OnSheetItemClickListener(){
        @Override
        public void onClick (int which){

        }
    })
    .show();
```

```
   Copyright 2016 imtiaanx

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```
