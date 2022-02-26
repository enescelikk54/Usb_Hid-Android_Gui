# USB HID stm32f401ccu6(BlackPill) + Android GUI

![github-small](https://github.com/sangariuss/Usb_Hid-Android_Gui/blob/main/github_android_otg_stm32.jpg)


1. Firmware Tarafı
- Stm32CubeIDE kullanarak HAL kütüphaneleri ile yapacağız.
- IOC ayarlarını tek tek yazıyorum.
  
  RCC--> HSE   --> Crystal/Ceramic Resonator
  SYS--> Debug --> Serial Wire (Stlink ile debug edebilmek için gerekli)
  Connectivity
  USB_OTG_FS --> Mode --> Device Only + NVIC Settings --> USB On The Go FS global İnterrupti Enable Et.
  Middleware
  USB_DEVICE --> Class For FS IP --> Custom Human Interface 
                 sekmesinde Device Descriptordeki bilgilere 
                 bakınız.
  
  
  
   





2. Software Tarafı
