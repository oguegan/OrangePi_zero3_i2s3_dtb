# Orangepi_Zero3 linux 6.1 user overlay for i2s3

This is a user overlay for configuring pins PH5, PH6, PH7, PH8 and PH9 as I2S3 interface for kernel linux 6.1 (orangepi linux specific for Orange pi Zero3 board)

PH5<=>MCLK
PH6<=>BCLK
PH7<=>LRCK
PH8<=>Data Out
PH9<=>Data In

NOTE : for connecting a pcm5102a i2s card/module, only PH6, PH7, PH8 are needed

once loaded, in alsamixer, need to configure outputcard "ahubdam" to set i2s3 source on APBIF_TX2

the pcm card itself is "ahubi2s3"

should be listed under "aplay -l"

can be tested with "speaker-test -Ddefault:ahubi2s3 -c 2"



