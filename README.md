# rpi-zero-slideshow

Raspberry Pi OS-lite
SSH with key
WIFI
WIFI region
Locale

sudo apt update
sudo apt upgrade -y
sudo apt install fbi imagemagick -y

sudo raspi-config

-- auto login cli

Add to .bashrc for user:pi

export FRAMEBUFFER=/dev/fb0
export DISPLAY=:0
sudo /usr/bin/fbi -a -u --noverbose -T 1 -t 10 /home/pi/Pictures/*.jpg &

wget https://downloads.rclone.org/rclone-current-linux-arm.zip
unzip -j -d rclone-temp rclone-current-linux-arm.zip
sudo install rclone-temp/rclone /usr/local/bin

rm ~/rclone-current-linux-arm.zip
rm -r -f ~/rclone-temp
