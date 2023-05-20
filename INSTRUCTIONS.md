# Flash-Rom--
Flash ROM 
## INSTRUCTIONS FOR FLASHING ROMS IN ASTRO VIA FASTBOOTD

# For Clean Flash

fastboot reboot fastboot

fastboot set_active a

fastboot -w

fastboot delete-logical-partition system_a

fastboot delete-logical-partition product_a

fastboot create-logical-partition system_a 1

fastboot create-logical-partition product_a 1

fastboot flash boot boot.img

fastboot flash dtbo dtbo.img

fastboot flash system system.img

fastboot flash product product.img

fastboot flash vendor vendor.img

fastboot flash vbmeta vbmeta.img

fastboot reboot

# For Dirty Flash

fastboot reboot fastboot

fastboot set_active a

fastboot flash system system.img

fastboot flash product product.img

fastboot flash vendor vendor.img

fastboot flash vbmeta vbmeta.img

fastboot reboot
