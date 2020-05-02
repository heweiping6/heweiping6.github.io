### pl2303

http://www.prolific.com.tw/us/showproduct.aspx?p_id=229&pcid=41

http://www.prolific.com.tw/UserFiles/files/PL2303HXD_G_Driver_v2_0_0_20191204.zip

unzip the package

read the install guide and follow it

reboot the system


### minicom

http://archive.ubuntu.com/ubuntu/pool/universe/m/minicom/minicom_2.7.1.orig.tar.gz

```bash
./configure  --prefix=$HEWEIPING6/minicom
make install
mkdir -p $HEWEIPING6/minicom/etc
#plugin the pl2303
minicom -s
#set port to cu.usbserial
```
