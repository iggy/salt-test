salt-test
=========

To use:

cat >/etc/salt/master.d/fileserver.conf <<EOF
fileserver_backend:
  - git

gitfs_remotes:
  - git@github.com:iggy/salt-test.git:
    - root: srv/salt
EOF
