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
