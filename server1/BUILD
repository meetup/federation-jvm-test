java_binary(
    name = "server1",
    srcs = glob(["src/main/java/com/meetup/graphql/federation/*.java"]),
    main_class = "com.meetup.graphql.federation.App",
    resources = ["src/main/resources/inventory.graphql"],
    deps = [
        "@maven//:com_apollographql_federation_federation_graphql_java_support",
        "@maven//:org_springframework_spring_core",
        "@maven//:org_springframework_spring_context",
        "@maven//:org_springframework_spring_beans",
        "@maven//:org_springframework_boot_spring_boot",
        "@maven//:org_springframework_boot_spring_boot_autoconfigure",
        "@maven//:org_springframework_boot_spring_boot_starter_actuator",
        "@maven//:org_springframework_boot_spring_boot_starter_web",
        "@maven//:com_graphql_java_kickstart_graphql_spring_boot_starter",
        "@maven//:com_graphql_java_kickstart_graphql_java_servlet",
        "@maven//:org_jetbrains_annotations",
    ],
)