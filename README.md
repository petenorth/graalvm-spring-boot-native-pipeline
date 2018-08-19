THIS IS WORK IN PROGRESS 

CURRENTLY GIVES AN ERROR AT POD START UP

Anyway to get started utilize the generic GraalVM Native Image pipeline template

    oc process -f https://raw.githubusercontent.com/petenorth/graalvm-native-maven-template/master/graalvm-native-maven-template.yaml \
      -p GIT_REPO=https://github.com/petenorth/graalvm-spring-boot-native-pipeline.git \
      -p GIT_BRANCH=master \
      -p APP_NAME=test | oc create -f -
