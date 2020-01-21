# Description:
#   Kafka C/C++ (librdkafka) client library

licenses(["notice"])  # 2-clause BSD license

exports_files(["LICENSE"])

cc_library(
    name = "kafka",
    srcs = [
        "config.h",
        "src-cpp/ConfImpl.cpp",
        "src-cpp/ConsumerImpl.cpp",
        "src-cpp/HandleImpl.cpp",
        "src-cpp/KafkaConsumerImpl.cpp",
        "src-cpp/MessageImpl.cpp",
        "src-cpp/MetadataImpl.cpp",
        "src-cpp/ProducerImpl.cpp",
        "src-cpp/QueueImpl.cpp",
        "src-cpp/RdKafka.cpp",
        "src-cpp/TopicImpl.cpp",
        "src-cpp/TopicPartitionImpl.cpp",
        "src/crc32c.c",
        "src/crc32c.h",
        "src/lz4.c",
        "src/lz4.h",
        "src/lz4frame.c",
        "src/lz4frame.h",
        "src/lz4frame_static.h",
        "src/lz4hc.c",
        "src/lz4hc.h",
        "src/lz4opt.h",
        "src/queue.h",
        "src/rd.h",
        "src/rdaddr.c",
        "src/rdaddr.h",
        "src/rdatomic.h",
        "src/rdavg.h",
        "src/rdavl.c",
        "src/rdavl.h",
        "src/rdbuf.c",
        "src/rdbuf.h",
        "src/rdcrc32.h",
        "src/rddl.h",
        "src/rdendian.h",
        "src/rdgz.c",
        "src/rdgz.h",
        "src/rdinterval.h",
        "src/rdkafka.c",
        "src/rdkafka.h",
        "src/rdkafka_admin.c",
        "src/rdkafka_admin.h",
        "src/rdkafka_assignor.c",
        "src/rdkafka_assignor.h",
        "src/rdkafka_aux.c",
        "src/rdkafka_aux.h",
        "src/rdkafka_background.c",
        "src/rdkafka_broker.c",
        "src/rdkafka_broker.h",
        "src/rdkafka_buf.c",
        "src/rdkafka_buf.h",
        "src/rdkafka_cgrp.c",
        "src/rdkafka_cgrp.h",
        "src/rdkafka_conf.c",
        "src/rdkafka_conf.h",
        "src/rdkafka_confval.h",
        "src/rdkafka_event.h",
        "src/rdkafka_feature.c",
        "src/rdkafka_feature.h",
        "src/rdkafka_header.c",
        "src/rdkafka_header.h",
        "src/rdkafka_int.h",
        "src/rdkafka_interceptor.c",
        "src/rdkafka_interceptor.h",
        "src/rdkafka_lz4.c",
        "src/rdkafka_lz4.h",
        "src/rdkafka_metadata.c",
        "src/rdkafka_metadata.h",
        "src/rdkafka_metadata_cache.c",
        "src/rdkafka_msg.c",
        "src/rdkafka_msg.h",
        "src/rdkafka_msgset.h",
        "src/rdkafka_msgset_reader.c",
        "src/rdkafka_msgset_writer.c",
        "src/rdkafka_offset.c",
        "src/rdkafka_offset.h",
        "src/rdkafka_op.c",
        "src/rdkafka_op.h",
        "src/rdkafka_partition.c",
        "src/rdkafka_partition.h",
        "src/rdkafka_pattern.c",
        "src/rdkafka_pattern.h",
        "src/rdkafka_proto.h",
        "src/rdkafka_queue.c",
        "src/rdkafka_queue.h",
        "src/rdkafka_range_assignor.c",
        "src/rdkafka_request.c",
        "src/rdkafka_request.h",
        "src/rdkafka_roundrobin_assignor.c",
        "src/rdkafka_sasl.c",
        "src/rdkafka_sasl.h",
        "src/rdkafka_sasl_int.h",
        "src/rdkafka_sasl_plain.c",
        "src/rdkafka_subscription.c",
        "src/rdkafka_timer.c",
        "src/rdkafka_timer.h",
        "src/rdkafka_topic.c",
        "src/rdkafka_topic.h",
        "src/rdkafka_transport.c",
        "src/rdkafka_transport.h",
        "src/rdkafka_transport_int.h",
        "src/rdlist.c",
        "src/rdlist.h",
        "src/rdlog.c",
        "src/rdlog.h",
        "src/rdmurmur2.c",
        "src/rdmurmur2.h",
        "src/rdports.c",
        "src/rdports.h",
        "src/rdposix.h",
        "src/rdrand.c",
        "src/rdrand.h",
        "src/rdregex.c",
        "src/rdregex.h",
        "src/rdstring.c",
        "src/rdstring.h",
        "src/rdsysqueue.h",
        "src/rdtime.h",
        "src/rdtypes.h",
        "src/rdunittest.c",
        "src/rdunittest.h",
        "src/rdvarint.c",
        "src/rdvarint.h",
        "src/snappy.c",
        "src/snappy.h",
        "src/tinycthread.c",
        "src/tinycthread.h",
        "src/tinycthread_extra.c",
        "src/tinycthread_extra.h",
    ],
    hdrs = [
        "config.h",
        "src-cpp/rdkafkacpp.h",
        "src-cpp/rdkafkacpp_int.h",
        "src/lz4.c",
        "src/snappy_compat.h",
    ],
    defines = ["LIBRDKAFKA_STATICLIB"],
    includes = [
        "src",
        "src-cpp",
    ],
    linkopts = ["-lpthread"],
    visibility = ["//visibility:public"],
    deps = [
        "@arrow",
        "@boringssl//:ssl",
        "@zlib",
    ],
)
