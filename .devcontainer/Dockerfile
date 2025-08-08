FROM ubuntu:24.04

ENV TZ=Asia/Tokyo
RUN <<EOF
ln -s /usr/share/zoneinfo/$TZ /etc/localtime
EOF

RUN <<EOF
apt update
apt install -y doxygen graphviz git git-lfs python3

EOF

RUN <<EOF
git config --global --add safe.directory /workspaces/MatterDocs/connectedhomeip
EOF