### 修改sde分区表
    我知道Android一共有大概6个磁盘sda,sdb,sdc,sdd,sde,sdf,sdg.<br />
    其中sda主要是misc,userdata,super,rescue和vbmeta_system系统校验分区的主要阵地,misc用于记录下次启动模式,userdata就是用户数据部分,super是系统镜像分区,rescue分区是紧急微系统分区(目前不清楚是什么界面)。userdata除了用户数据，还可以作为双系统的系统分区,只要对userdata再分盘就行,mipad5就是通过这种方式.<br />
    sdb是xbl_a磁盘,sdc是xbl_b磁盘,sdd目前不知道.<br />
    sde是引导分区,主要有boot_a/b,vbmeta_系统校验分区    我当初想对gpt分区表项进行修改,其中sde是引导磁盘