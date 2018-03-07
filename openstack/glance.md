# Glance CheatSheet

## List Images
glance image-list

## Delete Images
glance image-delete 788900aa-944c-451d-a237-18866a7d0b99

## Download Image
glance image-download --file < file name with ext > --progress < image id >

## Create Image
glance image-create --disk-format qcow2 --container-format bare --file CentOS-6-x86_64-GenericCloud-1707.qcow2 --visibility public --name "CentOS 6" --property description='CO6' --property virtual_size=760086528
