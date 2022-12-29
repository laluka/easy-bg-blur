# easy-bg-blur

A single-page tool to present your webcam with a blurred background.

# HowTo - Ubuntu

Simply open your browser and visit: `file:///opt/easy-bg-blur/index.html`

```bash
# Setup
sudo add-apt-repository ppa:obsproject/obs-studio
sudo apt update
sudo apt install v4l2loopback-dkms obs-studio

# Camera creation
sudo sed -i 's/Exec=obs/Exec=obs --use-fake-ui-for-media-stream/g' /usr/share/applications/com.obsproject.Studio.desktop
# Start OBS & create screne & virtual camera
```


# Kudos

- Original creator: https://usher.dev/posts/make-your-webcam-look-slightly-more-professional/
- Tech: https://github.com/tensorflow/tfjs-models/tree/master/body-pix