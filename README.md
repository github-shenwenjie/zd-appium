# ubuntu下appium环境搭建

安装JAVA

apt-get update

apt-get install openjdk-8-jre openjdk-8-jdk

java -version

设置环境变量：sudo gedit /etc/profile

export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64

export JRE_HOME=${JAVA_HOME}/jre 

export CLASSPATH=.:${JAVA_HOME}/lib:${JRE_HOME}/lib 

export PATH=${JAVA_HOME}/bin:$PATH

修改生效：source /etc/profile

验证：echo $JAVA_HOME


安装NODEJS

npm install -g n

n stable


安装AndroidSDK

下载https://developer.android.com/studio

android-studio/bin/ 目录，并执行 studio.sh

设置环境变量：sudo gedit /etc/profile

export ANDROID_HOME=/home/shenwenjie/Downloads/Android/Sdk

export PATH=$PATH:$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools:${JAVA_HOME}/bin

修改生效：source /etc/profile

验证：adb devices


安装appium

npm install -g appium

npm install -g appium-doctor

验证环境：appium-doctor
