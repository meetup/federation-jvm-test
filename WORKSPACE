
load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

RULES_JVM_EXTERNAL_TAG = "2.2"
RULES_JVM_EXTERNAL_SHA = "f1203ce04e232ab6fdd81897cf0ff76f2c04c0741424d192f28e65ae752ce2d6"

http_archive(
    name = "rules_jvm_external",
    strip_prefix = "rules_jvm_external-%s" % RULES_JVM_EXTERNAL_TAG,
    sha256 = RULES_JVM_EXTERNAL_SHA,
    url = "https://github.com/bazelbuild/rules_jvm_external/archive/%s.zip" % RULES_JVM_EXTERNAL_TAG,
)

load("@rules_jvm_external//:defs.bzl", "maven_install")

maven_install(
    name = "maven",
    artifacts = [
        "com.apollographql.federation:federation-graphql-java-support:0.2.0",
        "org.springframework:spring-core:5.1.8.RELEASE",
        "org.springframework:spring-context:5.1.8.RELEASE",
        "org.springframework:spring-beans:5.1.8.RELEASE",
        "org.springframework.boot:spring-boot:2.1.6.RELEASE",
        "org.springframework.boot:spring-boot-autoconfigure:2.1.6.RELEASE",
        "org.springframework.boot:spring-boot-starter-actuator:2.1.6.RELEASE",
        "org.springframework.boot:spring-boot-starter-web:2.1.6.RELEASE",
        "com.graphql-java-kickstart:graphql-spring-boot-starter:5.10.0",
        "com.graphql-java-kickstart:graphql-java-servlet:8.0.0",
        "org.jetbrains:annotations:17.0.0",
    ],
    repositories = [
        "https://jcenter.bintray.com/",
        "https://maven.google.com",
        "https://repo1.maven.org/maven2",
    ],
)