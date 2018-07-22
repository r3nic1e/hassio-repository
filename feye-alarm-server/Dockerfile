ARG BUILD_FROM
FROM $BUILD_FROM

ENV LANG C.UTF-8

ARG BUILD_VERSION
ADD https://github.com/r3nic1e/falcon-eye-alarm-server/releases/download/$BUILD_VERSION/feye_alarm_server.linux.arm64 /feye_alarm_server

COPY run.sh /
RUN chmod a+x /run.sh /feye_alarm_server

CMD /run.sh
