# bspatch
android patch update

//---------------------------------------------
//测试流程
//---------------------------------------------

//生成增量
bsdiff demo-old.apk demo-new.apk demo.patch
//将增量放到SD卡根目录
adb push demo.patch /sdcard/
//安装旧包进行安装
adb install demo-old.apk
//测试
。。。。。。
