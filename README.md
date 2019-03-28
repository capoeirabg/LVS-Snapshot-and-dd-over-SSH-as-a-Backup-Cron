#Creating an executable bash file per target for backup

touch $targetName.sh

chmod +X $targetName.sh

nano $targetName.sh

#Editing per target the nesecary variables

+lvcreate -L$sapshot_size(1G=1000M..) -s -n $Snapshot_name /dev/$VG_name/$LV_name &&
