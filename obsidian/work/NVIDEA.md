lspci | grep -i nvidia - она покажет, видит ли система сам PCI-e адаптер видеокарты.

nvidia-smi

sudo dmesg | grep NVRM

Какой драйвер привязан к каждому устройству PCI
lspci -nnk -d 10de:

удалите старый драйвер
sudo apt purge -y nvidia-*
sudo apt autoremove

рекомендуемый
ubuntu-drivers devices

установка 
sudo apt install nvidia-driver-570