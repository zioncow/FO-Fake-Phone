# mount_sd.py will mount an SD card volume
import board, busio, sdcardio, storage
# setup pins for SPI
sck = board.GP10
si = board.GP11
so = board.GP12
cs = board.GP13
spi = busio.SPI(sck, si, so)
sdcard = sdcardio.SDCard(spi, cs)
vfs = storage.vfsFat(sdcard)
storage.mount(vfs, "/sd")
