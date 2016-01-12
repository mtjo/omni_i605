MIUI patchrom i605 开源说明

安装环境
sudo apt-get install git-core gnupg flex bison gperf libsdl1.2-dev libesd0-dev libwxgtk2.8-dev squashfs-tools build-essential zip curl libncurses5-dev zlib1g-dev pngcrush schedtool libc6-dev x11proto-core-dev libx11-dev libreadline6-dev libgl1-mesa-dev g++-multilib mingw32 tofrodos python-markdown libxml2-utils xsltproc lib32ncurses5-dev lib32readline6-dev lib32z1-dev

cd ~/MIUI
repo init -u git://github.com/MiCode/patchrom.git -b miui-7 -m android-4.4.4.xml
repo sync
. build/envsetup.sh
cd I605
git clone git@github.com:mtjo/omni_i605.git
make fullota

