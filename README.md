# vmware-cheat-sheet




# Install

<br><br>

# Ubuntu
- https://support.broadcom.com/group/ecx/productfiles?subFamily=VMware%20Workstation%20Pro&displayGroup=VMware%20Workstation%20Pro%2017.0%20for%20Personal%20Use%20(Linux)&release=17.5.2&os=&servicePk=520450&language=EN
- If you can not install vmmon and vmnet download 17.5.1 and then:
```shell
wget https://github.com/mkubecek/vmware-host-modules/archive/workstation-17.5.1.tar.gz
tar -xzf workstation-17.5.1.tar.gz
cd vmware-host-modules-workstation-17.5.1/
tar -cf vmmon.tar vmmon-only
tar -cf vmnet.tar vmnet-only
sudo cp -v vmmon.tar vmnet.tar /usr/lib/vmware/modules/source/
sudo vmware-modconfig --console --install-all
```





<br><br>
<br><br>
_________________________
_________________________
<br><br>
<br><br>

# Troubleshooting

## Host os freezing
- When your host os is freezing randomly like 5- 10 minutes after you started your vm then try to disable 3d accelarition under the dsiplay tab
  - Or try also to icnrease the cpu processor
  - Or 
