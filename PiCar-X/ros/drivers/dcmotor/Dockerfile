ARG TAG=latest

FROM abarbie/picarx:${TAG}

COPY . ./src/drivers/dcmotor

RUN /bin/bash -c "source /opt/ros/noetic/setup.bash && catkin build"

ENTRYPOINT [ "/root/catkin_ws/src/arches/arches_core/ENTRYPOINT.sh" ]