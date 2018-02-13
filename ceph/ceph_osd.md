# ceph osd command cheatsheet

## Check OSD Disk Usage
- ceph osd df

## Check OSD Status
- ceph osd tree

## Get Quick Stats on OSDs
- ceph osd stat

## OSD Crush

## Reweight crush on an OSD
- ceph osd crush reweight [osd.#] [crush weight]
  - ceph osd crush reweight osd.10 0.0

## Place OSD in cluster
- ceph osd in [osd.#]
  - ceph osd in osd.1

## See status on OSD and what node it is on
- ceph osd status
