# Rascunho

Erro ao atualizar

![](img/firmware_missing0.gif)

W: Possible missing firmware /lib/firmware/i915/tgl_dmc_ver2_04.bin for module i915
W: Possible missing firmware /lib/firmware/i915/skl_guc_33.0.0.bin for module i915
W: Possible missing firmware /lib/firmware/i915/bxt_guc_33.0.0.bin for module i915
W: Possible missing firmware /lib/firmware/i915/kbl_guc_33.0.0.bin for module i915
W: Possible missing firmware /lib/firmware/i915/glk_guc_33.0.0.bin for module i915
W: Possible missing firmware /lib/firmware/i915/kbl_guc_33.0.0.bin for module i915
W: Possible missing firmware /lib/firmware/i915/icl_guc_33.0.0.bin for module i915

Baixando os firmwares

git clone https://git.kernel.org/pub/scm/linux/kernel/git/firmware/linux-firmware.git

Entrando no diretório

cd linux-firmware/i915/

Copiando cada um dos arquivos que faltam

sudo cp tgl_dmc_ver2_04.bin /lib/firmware/i915/
sudo cp skl_guc_33.0.0.bin /lib/firmware//i915/
sudo cp bxt_guc_33.0.0.bin /lib/firmware//i915/
sudo cp kbl_guc_33.0.0.bin /lib/firmware//i915/
sudo cp glk_guc_33.0.0.bin /lib/firmware//i915/
sudo cp kbl_guc_33.0.0.bin /lib/firmware//i915/
sudo cp icl_guc_33.0.0.bin /lib/firmware//i915/
