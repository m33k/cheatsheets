# ceph command cheatsheet

## Watch Ceph Activity
- ceph -w

## Check Ceph Disk Usage in Gigabyte
- ceph df

## Stop/Start all ceph mons and osds using targets
- systemctl stop ceph-mon.target (stop all monitors)
- systemctl start ceph-mon.target (start all monitors)
- systemctl stop ceph-osd.target (stop all osds)
- systemctl start ceph-osd.target (start all osds)

## Stop/Start ceph osd via /etc/init.d/ceph script
- /etc/init.d/ceph -a stop
- /etc/init.d/ceph -a start
- /etc/init.d/ceph -a stop
- /etc/init.d/ceph -a start
- /etc/init.d/ceph stop osd.12
- /etc/init.d/ceph stop osd.13

