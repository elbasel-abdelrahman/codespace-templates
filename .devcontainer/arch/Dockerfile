# Use the latest Arch Linux base image
FROM archlinux:multilib-devel

# Install other necessary packages

RUN pacman-key --init && \
    pacman-key --populate archlinux && \
    pacman -Sy --needed --noconfirm --disable-download-timeout archlinux-keyring && \
    pacman -Su --noconfirm --disable-download-timeout

RUN pacman -S --noconfirm git vim python zsh
