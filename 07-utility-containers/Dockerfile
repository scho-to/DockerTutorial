FROM node:14-slim
ARG USER_ID
ARG GROUP_ID
RUN userdel -r node
# RUN addgroup --gid $GROUP_ID user
RUN adduser --disabled-password --gecos '' --uid $USER_ID --gid $GROUP_ID user
USER user
WORKDIR /app

ENTRYPOINT [ "npm" ]