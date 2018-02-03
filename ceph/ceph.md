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
