# zd-appium

1. install java

   sudo apt-get update

   sudo apt-get install openjdk-8-jdk

   查看java路径： sudo update-alternatives --config java

   编辑 nano /etc/profile

   export JAVA_HOME="/usr/lib/jvm/java-8-openjdk-armhf/jre/bin/java"
    
   export PATH=${JAVA_HOME}/bin:$PATH

   生效 source /etc/profile

2. install node

   apt install npm

   npm install -g n

   n stable

3. install android sdk

   export ANDROID_HOME="/root/android-sdk-linux"
   
   export ANDROID_SWT="/root/android-sdk-linux/tools/lib/x86_64/"

   export PATH="${JAVA_HOME}/bin:$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools:$PATH"
   
   PATH="$PATH:$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools"

   sudo add-apt-repository ppa:nilarimogard/webupd8
  
   sudo apt-get update
  
   sudo apt-get install android-tools-adb android-tools-fastboot

   cp /usr/bin/adb /root/android-sdk-linux/platform-tools/adb

3. install appium

   npm install -g appium --unsafe-perm=true --allow-root

   npm install -g appium-doctor

