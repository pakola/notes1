

nvidia-open-dkms 


nvidia_drm.modeset=1  /boot/loader/entries/arch.conf



sudo mkinitcpio --config /etc/mkinitcpio.conf --generate /boot/initramfs-custom.img




run # mkinitcpio --config /etc/mkinitcpio.conf --generate /boot/initramfs-custom.img (make sure you have the linux-headers package installed first)



env = LIBVA_DRIVER_NAME,nvidia
env = XDG_SESSION_TYPE,wayland
env = GBM_BACKEND,nvidia-drm
env = __GLX_VENDOR_LIBRARY_NAME,nvidia
env = WLR_NO_HARDWARE_CURSORS,1





  kitty 
    mako 
    waybar-hyprland 
    swww 
    swaylock-effects 
    wofi 
    wlogout 
    xdg-desktop-portal-hyprland 
    swappy 
    grim 
    slurp 
    thunar 
    btop
    firefox
    thunderbird
    mpv
    pamixer 
    pavucontrol 
    brightnessctl 
    bluez 
    bluez-utils 
    blueman 
    network-manager-applet 
    gvfs 
    thunar-archive-plugin 
    file-roller
    starship 
    papirus-icon-theme 
    ttf-jetbrains-mono-nerd 
    noto-fonts-emoji 
    lxappearance 
    xfce4-settings
    nwg-look-bin
    sddm-git 
    sddm-sugar-candy-git
    
    
    to install yay 
    git clone https://aur.archlinux.org/yay.git &>> $INSTLOG
    cd yay
    makepkg -si 
    
    
    
    git clone --recursive https://github.com/hyprwm/Hyprland
cd Hyprland
sudo make install
