ARG ST2_VERSION
FROM registry.cn-beijing.aliyuncs.com/zhouys/st2common:v1.0
#FROM stackstorm/st2:${ST2_VERSION}
LABEL com.stackstorm.component="st2rulesengine"

USER st2

CMD ["/opt/stackstorm/st2/bin/st2rulesengine", "--config-file=/etc/st2/st2.conf", "--config-file=/etc/st2/st2.docker.conf", "--config-file=/etc/st2/st2.user.conf"]
