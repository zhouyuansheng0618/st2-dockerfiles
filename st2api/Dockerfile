ARG ST2_VERSION
FROM registry.cn-beijing.aliyuncs.com/zhouys/st2common:v1.0
#FROM stackstorm/st2:${ST2_VERSION}
LABEL com.stackstorm.component="st2api"

USER st2

VOLUME ["/etc/st2/keys", "/opt/stackstorm/rbac"]
CMD ["/opt/stackstorm/st2/bin/st2api", "--config-file=/etc/st2/st2.conf", "--config-file=/etc/st2/st2.docker.conf", "--config-file=/etc/st2/st2.user.conf"]
EXPOSE 9101
