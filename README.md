# BH-A10AME 升级固件以支持 UHD 功能指南 / Firmware Upgrade Guide for BH-A10AME (Enable UHD Support)


HL 出品的 BH-A10AME 是一款由紫晶储存定制的 BDXL 刻录机，基于 MT1959 平台，其硬件配置与 AUAS BW-16D1HT 一模一样。

由于紫晶专有固件的限制，BH-A10AME 可以刻录紫晶定制的三菱 100GB BDXL 蓝光碟，但是代价是失去了 UHD 读取能力，虽然是 2020 年的产品，却只支持 AACS v62 加密，这将导致其无法识别所有的 UHD 电影碟。

好消息是，我们可以通过将其刷入 AUAS BW-16D1HT 的固件来使其具有 UHD 读写能力。如果您在某些中国购物网站购买了该产品并且您只有一个蓝光光驱，这个方法可以让你不用再去购买额外的光驱来读取 UHD 电影碟。

**注意事项：**  
- 本方案只适用于 Windows 系统  
- 不适用于使用 SATA 转 USB 的笔记本用户  
- 支持 MakeMKV 的完整功能

**操作步骤如下：**

1. 在以下链接下载最新版的 **SDFtool.Flasher**：  
   https://github.com/hny3494317690/BH-A10AME/releases  
2. 下载固件文件：  
   https://github.com/hny3494317690/BH-A10AME/blob/main/ASUS-BW-16D1HT-3.10-WM01601-211901041014.bin  
3. 保持光驱连接电脑，并取出光盘  
4. 打开 SDFtool.Flasher，在下拉栏中选择 BH-A10AME，右侧选择 "Read FW"，点击 "Start"，耐心等待完成  
5. 在软件根目录的 `Firmware_Dumps` 文件夹下找到备份的固件文件并妥善保存  
6. 在软件窗口右侧选择 "RECOVER Drive"，在弹出的文件管理器中选择下载的固件文件，点击 "Start"  
7. 等待刷写完成后重启电脑  
8. 现在可以正常读取 UHD 电影碟了

---


The BH-A10AME by HL is a custom BDXL Blu-ray burner designed specifically for Zijing Storage. It's built on the MT1959 platform and has identical hardware to the ASUS BW-16D1HT.

Due to Zijing’s proprietary firmware, the BH-A10AME can burn Zijing-branded Mitsubishi 100GB BDXL discs. However, the trade-off is that it loses UHD playback support. Although it was released in 2020, it only supports AACS version 62 encryption, meaning it can’t read any UHD movie discs.

The good news is, you can flash the drive with ASUS BW-16D1HT firmware to unlock UHD read/write capabilities. If you bought this drive from certain Chinese online retailers and only have one Blu-ray drive, this method can save you from needing to buy another drive just to read UHD discs.

**Important Notes:**  
- This process only works on Windows  
- It does *not* work with SATA-to-USB adapters (such as in many laptops)  
- The drive will fully support MakeMKV's UHD features after flashing

**Steps to Flash the Firmware:**

1. Download the latest version of **SDFtool.Flasher** from:  
   https://github.com/hny3494317690/BH-A10AME/releases  
2. Download the ASUS BW-16D1HT firmware file from:  
   https://github.com/hny3494317690/BH-A10AME/blob/main/ASUS-BW-16D1HT-3.10-WM01601-211901041014.bin  
3. Keep your drive connected to the PC and remove any discs from the tray  
4. Open **SDFtool.Flasher**, select “BH-A10AME” from the dropdown, choose “Read FW” on the right, and click **Start**  
5. A backup of your current firmware will be saved under the `Firmware_Dumps` folder. Keep it safe in case you need to restore  
6. Select “RECOVER Drive” in the tool, choose the downloaded firmware file, and click **Start**  
7. Wait for the flashing process to complete, then restart your computer  
8. Your drive should now be able to read UHD movie discs normally