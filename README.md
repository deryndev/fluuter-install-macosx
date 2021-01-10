# fluuter-install-macosx

// .zshrc file

export PATH="$PATH:$HOME/<YOUR_UNZIP_PATH>/flutter/bin"

export ANDROID_SDK_ROOT=$HOME/<YOUR_ANDROID_SDK_PATH>

export ANDROID_HOME=$ANDROID_SDK_ROOT/tools

export PATH=$PATH:$ANDROID_SDK_ROOT/cmdline-tools/bin


________________________________________________________

// COMMAND LINE

sudo gem install cocoapods 

sdkmanager --sdk_root=$ANDROID_SDK_ROOT 
sdkmanager --sdk_root=$ANDROID_SDK_ROOT "platform-tools" "platforms;android-30" 
sdkmanager --sdk_root=$ANDROID_SDK_ROOT "build-tools;29.0.3" 
sdkmanager --sdk_root=$ANDROID_SDK_ROOT --install "ndk;22.0.7026061"

flutter config --android-sdk  $ANDROID_SDK_ROOT

flutter doctor --android-licenses  
