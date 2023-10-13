FROM quay.io/devfile/universal-developer-image:ubi8-latest

USER 10001

# set up pnpm
RUN \
    corepack enable \
    corepack prepare pnpm@latest --activate \
    SHELL=bash pnpm setup

WORKDIR /projects
CMD ["tail", "-f", "/dev/null"]