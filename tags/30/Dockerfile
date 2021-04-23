FROM androidsdk/android-30 as android

FROM node:15.11

COPY --from=android /usr/lib/jvm/java-8-openjdk-amd64 /usr/lib/jvm/java-8-openjdk-amd64

COPY --from=android /opt/android-sdk-linux /opt/android-sdk-linux

ENV ANDROID_HOME=/opt/android-sdk-linux

ENV ANDROID_SDK=/opt/android-sdk-linux

ENV ANDROID_SDK_HOME=/opt/android-sdk-linux

ENV ANDROID_SDK_ROOT=/opt/android-sdk-linux

ENV JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64

ENV JDK_HOME=/usr/lib/jvm/java-8-openjdk-amd64

ENV PATH=$JAVA_HOME/bin:$ANDROID_HOME/emulator:$ANDROID_HOME/tools:$ANDROID_HOME/tools/bin:$ANDROID_HOME/platform-tools:$PATH