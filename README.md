# UBI_postgresql_server
dnf install https://download.postgresql.org/pub/repos/yum/15/redhat/rhel-9-x86_64/postgresql15-libs-15.1-1PGDG.rhel9.x86_64.rpm -y

dnf install https://download.postgresql.org/pub/repos/yum/15/redhat/rhel-9-x86_64/postgresql15-15.1-1PGDG.rhel9.x86_64.rpm -y

dnf install https://download.postgresql.org/pub/repos/yum/15/redhat/rhel-9-x86_64/postgresql15-server-15.1-1PGDG.rhel9.x86_64.rpm -y

su postgres

/usr/pgsql-15/bin/initdb -D /var/lib/pgsql/15/data/

/usr/pgsql-15/bin/pg_ctl -D /var/lib/pgsql/15/data/ -l logfile start
