# rEFInd theme Regular

A simplistic clean and minimal theme for rEFInd


![Screenshot 01](https://i.imgur.com/foKbI3Q.png)
**press F10 to take screenshot


### Installation:

1. Clone git repository to your $HOME directory.
   ```
   git clone https://github.com/munlik/refind-theme-regular.git
   ```

2. Locate refind directory under EFI partition. For most Linux based system is commonly `/boot/efi/EFI/refind/`. Copy theme directory to it.

   **Important:** Delete older installed versions of this theme before you proceed any further.

   ```
   sudo rm -rf /boot/efi/EFI/refind/{regular-theme,refind-theme-regular}
   ```
   ```
   sudo cp -r refind-theme-regular /boot/efi/EFI/refind/
   ```
3. Remove unused directory.
   ```
   sudo rm -rf /boot/efi/EFI/refind/refind-theme-regular/{src,.git}
   ```

4. To adjust icon size and font size edit `theme.conf`.
   ```
   sudo nano /boot/efi/EFI/refind/refind-theme-regular/theme.conf
   ```

5. To enable the theme add `include refind-theme-regular/theme.conf` at the end of `refind.conf`.
   ```
   sudo nano /boot/efi/EFI/refind/refind.conf
   ```

**More information**

[rEFInd](http://www.rodsbooks.com/refind/) An official rEFInd website

## Modified

* `selection_big.png` and `selection_small.png` 
  * Based on the [rEFInd OS X theme](https://www.deviantart.com/naymlezwun/art/rEFInd-OS-X-Theme-469807750) created by: naymlexwun

* `os_kali.png`
  * From [PhineasPhreak](https://github.com/PhineasPhreak)'s avatar

* `refind.conf`
  * Change settings: timeout, hideui, showtools, dont_scan_dirs, default_selection and include `theme.conf`

* `refind_linux.conf`
  * conf for my old laptop