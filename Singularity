Bootstrap: docker
From: registry.gitlab.com/rode0day/fuzzer-testing/honggfuzz_runner:rolling

%labels
    MAINTAINER Josh Bundt
    DockerTagID e5f4112a9

%environment
    AFL_SKIP_CPUFREQ=1
    LC_ALL=C
    LANG=C
    export AFL_SKIP_CPUFREQ LC_ALL LANG

%runscript
    exec /start_fuzzing "$@"

