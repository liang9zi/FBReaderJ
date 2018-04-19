ROM xujianliang/android_ci_sdk:v1.0
MAINTAINER xujianliang <xujianliang@163.com>
ENV PROJECT /project
RUN mkdir $PROJECT
WORKDIR $PROJECT
ADD . $PROJECT
RUN chmod +x ./gradlew
RUN echo "sdk.dir=$ANDROID_HOME" > local.properties && \
./gradlew --stacktrace app:dependencies
