# snapper-rollback
Um script para criar um snapshot também das partições /boot e /boot/efi no Fedora linux. 
O proposíto é facilitar a transição para snapshots criados pelo btrfs-assistant, sem perder
o boot do sistema, ele funciona com a partição raiz criptografada.

# ATENÇÃO
> Esse script é útil numa instalação a qual o btrfs-assistant não foi configurado, pois o script precisa ser executado primeiramente antes que qualquer 
snapshot seja criado, a fim de iniciar o backup do diretório /boot e /boot/efi.

> É UM SCRIPT FEITO POR UMA PESSOA SÓ, NÃO FOI AMPLAMENTE TESTADO, PORTANTO USE POR SUA CONTA E RISCO EM PRODUÇÃO!!!!

# Pacotes necessários 
```
sudo dnf install libdnf5-plugin-actions btrfs-assistant
```
# Instação 
```
git clone https://github.com/Ferlinuxdebian/snapper-rollback.git
```

```
cd snapper-rollback; chmod +x snapper-rollback; sudo mv snapper-rollback /usr/local/bin/
```

# Video de desmostração do software
