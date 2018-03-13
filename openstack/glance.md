# Glance CheatSheet

## List Images
glance image-list

## Delete Images
glance image-delete 788900aa-944c-451d-a237-18866a7d0b99

## Download Image
glance image-download --file < file name with ext > --progress < image id >

## Create Image
glance image-create --disk-format qcow2 --container-format bare --file CentOS-6-x86_64-GenericCloud-1707.qcow2 --visibility public --name "CentOS 6" --property description='CO6' --property virtual_size=760086528

## Show Details About Image
glance image-show f630811a-b59b-4c0b-b235-1b1a6375bafe

## Protect and UnProtect Image
glance image-update --protected True 26930a38-42b9-4698-8102-8f3f5766acb8
glance image-update --protected False 26930a38-42b9-4698-8102-8f3f5766acb8

## Rename an image
glance image-update --name "$NEW_NAME" de35d4da-41e7-4298-bbb4-855bdb2380ee
