# An epic filesystem quest
## INTRODUCTION 
In the ninth task, we need to find a hidden flag using the knowledge of `cd`,` ls`, and` cat`, I `cd` to `/` and then found clue to get to the flag.
## CODE
``` bash
Connected!
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
BLUEPRINT  bin  boot  challenge  dev  etc  flag  home  lib  lib32  lib64  libx32  media  mnt  nix  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
hacker@commands~an-epic-filesystem-quest:/$ cat BLUEPRINT
Congratulations, you found the clue!
The next clue is in: /opt/linux/linux-5.4/drivers/net/wireless/realtek/rtlwifi/rtl8723be

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/$ ls /opt/linux/linux-5.4/drivers/net/wireless/realtek/rtlwifi/rtl8723be
CUE-TRAPPED  Makefile  def.h  dm.c  dm.h  fw.c  fw.h  hw.c  hw.h  led.c  led.h  phy.c  phy.h  pwrseq.c  pwrseq.h  reg.h  rf.c  rf.h  sw.c  sw.h  table.c  table.h  trx.c  trx.h
hacker@commands~an-epic-filesystem-quest:/$ cat /opt/linux/linux-5.4/drivers/net/wireless/realtek/rtlwifi/rtl8723be/CUE-TRAPPED
Congratulations, you found the clue!
The next clue is in: /usr/share/javascript/mathjax/unpacked/jax/output/SVG/fonts/Asana-Math/Fraktur/Regular

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/share/javascript/mathjax/unpacked/jax/output/SVG/fonts/Asana-Math/Fraktur/Regular
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/jax/output/SVG/fonts/Asana-Math/Fraktur/Regular$ ls -a
.  ..  .CLUE  Main.js
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/jax/output/SVG/fonts/Asana-Math/Fraktur/Regular$ cat .CLUE
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/drivers/misc/sgi-xp
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/jax/output/SVG/fonts/Asana-Math/Fraktur/Regular$ cd /opt/linux/linux-5.4/drivers/misc/sgi-xp
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/misc/sgi-xp$ ls
Makefile  TIP  xp.h  xp_main.c  xp_uv.c  xpc.h  xpc_channel.c  xpc_main.c  xpc_partition.c  xpc_uv.c  xpnet.c
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/misc/sgi-xp$ cat TIP
Yahaha, you found me!
The next clue is in: /usr/lib/firefox/browser/chrome

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/misc/sgi-xp$ cd /usr/lib/firefox/browser/chrome
hacker@commands~an-epic-filesystem-quest:/usr/lib/firefox/browser/chrome$ ls -a
.  ..  .POINTER  icons
hacker@commands~an-epic-filesystem-quest:/usr/lib/firefox/browser/chrome$ cat .POINTER
Tubular find!
The next clue is in: /usr/lib/python3/dist-packages/setuptools/_vendor/packaging

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/lib/firefox/browser/chrome$ ls /usr/lib/python3/dist-packages/setuptools/_vendor/packaging
DOSSIER-TRAPPED  __about__.py  __init__.py  __pycache__  _compat.py  _structures.py  markers.py  requirements.py  specifiers.py  tags.py  utils.py  version.py
hacker@commands~an-epic-filesystem-quest:/usr/lib/firefox/browser/chrome$ cat /usr/lib/python3/dist-packages/setuptools/_vendor/packaging/DOSSIER-TRAPPED
Great sleuthing!
The next clue is in: /usr/share/ca-certificates/mozilla

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/firefox/browser/chrome$ cd /usr/share/ca-certificates/mozilla
hacker@commands~an-epic-filesystem-quest:/usr/share/ca-certificates/mozilla$ ls
 ACCVRAIZ1.crt                                                     DigiCert_Trusted_Root_G4.crt                                      QuoVadis_Root_CA_3.crt
 AC_RAIZ_FNMT-RCM.crt                                              E-Tugra_Certification_Authority.crt                               QuoVadis_Root_CA_3_G3.crt
 AC_RAIZ_FNMT-RCM_SERVIDORES_SEGUROS.crt                           E-Tugra_Global_Root_CA_ECC_v3.crt                                 SSL.com_EV_Root_Certification_Authority_ECC.crt
 ANF_Secure_Server_Root_CA.crt                                     E-Tugra_Global_Root_CA_RSA_v3.crt                                 SSL.com_EV_Root_Certification_Authority_RSA_R2.crt
 Actalis_Authentication_Root_CA.crt                                Entrust.net_Premium_2048_Secure_Server_CA.crt                     SSL.com_Root_Certification_Authority_ECC.crt
 AffirmTrust_Commercial.crt                                        Entrust_Root_Certification_Authority.crt                          SSL.com_Root_Certification_Authority_RSA.crt
 AffirmTrust_Networking.crt                                        Entrust_Root_Certification_Authority_-_EC1.crt                    SZAFIR_ROOT_CA2.crt
 AffirmTrust_Premium.crt                                           Entrust_Root_Certification_Authority_-_G2.crt                     SecureSign_RootCA11.crt
 AffirmTrust_Premium_ECC.crt                                       Entrust_Root_Certification_Authority_-_G4.crt                     SecureTrust_CA.crt
 Amazon_Root_CA_1.crt                                              GDCA_TrustAUTH_R5_ROOT.crt                                        Secure_Global_CA.crt
 Amazon_Root_CA_2.crt                                              GLOBALTRUST_2020.crt                                              Security_Communication_ECC_RootCA1.crt
 Amazon_Root_CA_3.crt                                              GTS_Root_R1.crt                                                   Security_Communication_RootCA2.crt
 Amazon_Root_CA_4.crt                                              GTS_Root_R2.crt                                                   Security_Communication_RootCA3.crt
 Atos_TrustedRoot_2011.crt                                         GTS_Root_R3.crt                                                   Security_Communication_Root_CA.crt
 Autoridad_de_Certificacion_Firmaprofesional_CIF_A62634068.crt     GTS_Root_R4.crt                                                   Starfield_Class_2_CA.crt
 Autoridad_de_Certificacion_Firmaprofesional_CIF_A62634068_2.crt   GlobalSign_ECC_Root_CA_-_R4.crt                                   Starfield_Root_Certificate_Authority_-_G2.crt
 Baltimore_CyberTrust_Root.crt                                     GlobalSign_ECC_Root_CA_-_R5.crt                                   Starfield_Services_Root_Certificate_Authority_-_G2.crt
 Buypass_Class_2_Root_CA.crt                                       GlobalSign_Root_CA.crt                                            SwissSign_Gold_CA_-_G2.crt
 Buypass_Class_3_Root_CA.crt                                       GlobalSign_Root_CA_-_R3.crt                                       SwissSign_Silver_CA_-_G2.crt
 CA_Disig_Root_R2.crt                                              GlobalSign_Root_CA_-_R6.crt                                       T-TeleSec_GlobalRoot_Class_2.crt
 CFCA_EV_ROOT.crt                                                  GlobalSign_Root_E46.crt                                           T-TeleSec_GlobalRoot_Class_3.crt
 COMODO_Certification_Authority.crt                                GlobalSign_Root_R46.crt                                           TUBITAK_Kamu_SM_SSL_Kok_Sertifikasi_-_Surum_1.crt
 COMODO_ECC_Certification_Authority.crt                            Go_Daddy_Class_2_CA.crt                                           TWCA_Global_Root_CA.crt
 COMODO_RSA_Certification_Authority.crt                            Go_Daddy_Root_Certificate_Authority_-_G2.crt                      TWCA_Root_Certification_Authority.crt
 Certainly_Root_E1.crt                                             HARICA_TLS_ECC_Root_CA_2021.crt                                   TeliaSonera_Root_CA_v1.crt
 Certainly_Root_R1.crt                                             HARICA_TLS_RSA_Root_CA_2021.crt                                   Telia_Root_CA_v2.crt
 Certigna.crt                                                      Hellenic_Academic_and_Research_Institutions_ECC_RootCA_2015.crt   Trustwave_Global_Certification_Authority.crt
 Certigna_Root_CA.crt                                              Hellenic_Academic_and_Research_Institutions_RootCA_2015.crt       Trustwave_Global_ECC_P256_Certification_Authority.crt
 Certum_EC-384_CA.crt                                              HiPKI_Root_CA_-_G1.crt                                            Trustwave_Global_ECC_P384_Certification_Authority.crt
 Certum_Trusted_Network_CA.crt                                     Hongkong_Post_Root_CA_1.crt                                       TunTrust_Root_CA.crt
 Certum_Trusted_Network_CA_2.crt                                   Hongkong_Post_Root_CA_3.crt                                       UCA_Extended_Validation_Root.crt
 Certum_Trusted_Root_CA.crt                                        ISRG_Root_X1.crt                                                  UCA_Global_G2_Root.crt
 Comodo_AAA_Services_root.crt                                      ISRG_Root_X2.crt                                                  USERTrust_ECC_Certification_Authority.crt
 D-TRUST_BR_Root_CA_1_2020.crt                                     IdenTrust_Commercial_Root_CA_1.crt                                USERTrust_RSA_Certification_Authority.crt
 D-TRUST_EV_Root_CA_1_2020.crt                                     IdenTrust_Public_Sector_Root_CA_1.crt                             WHISPER
 D-TRUST_Root_Class_3_CA_2_2009.crt                                Izenpe.com.crt                                                    XRamp_Global_CA_Root.crt
 D-TRUST_Root_Class_3_CA_2_EV_2009.crt                             Microsec_e-Szigno_Root_CA_2009.crt                                certSIGN_ROOT_CA.crt
 DigiCert_Assured_ID_Root_CA.crt                                   Microsoft_ECC_Root_Certificate_Authority_2017.crt                 certSIGN_Root_CA_G2.crt
 DigiCert_Assured_ID_Root_G2.crt                                   Microsoft_RSA_Root_Certificate_Authority_2017.crt                 e-Szigno_Root_CA_2017.crt
 DigiCert_Assured_ID_Root_G3.crt                                   NAVER_Global_Root_Certification_Authority.crt                     ePKI_Root_Certification_Authority.crt
 DigiCert_Global_Root_CA.crt                                      'NetLock_Arany_=Class_Gold=_Főtanúsítvány.crt'                     emSign_ECC_Root_CA_-_C3.crt
 DigiCert_Global_Root_G2.crt                                       OISTE_WISeKey_Global_Root_GB_CA.crt                               emSign_ECC_Root_CA_-_G3.crt
 DigiCert_Global_Root_G3.crt                                       OISTE_WISeKey_Global_Root_GC_CA.crt                               emSign_Root_CA_-_C1.crt
 DigiCert_High_Assurance_EV_Root_CA.crt                            QuoVadis_Root_CA_1_G3.crt                                         emSign_Root_CA_-_G1.crt
 DigiCert_TLS_ECC_P384_Root_G5.crt                                 QuoVadis_Root_CA_2.crt                                            vTrus_ECC_Root_CA.crt
 DigiCert_TLS_RSA4096_Root_G5.crt                                  QuoVadis_Root_CA_2_G3.crt                                         vTrus_Root_CA.crt
hacker@commands~an-epic-filesystem-quest:/usr/share/ca-certificates/mozilla$ cat WHISPER
Congratulations, you found the clue!
The next clue is in: /usr/share/icons/ubuntu-mono-dark/apps/48

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/ca-certificates/mozilla$ cd ^C
hacker@commands~an-epic-filesystem-quest:/usr/share/ca-certificates/mozilla$ cd /usr/share/icons/ubuntu-mono-dark/apps/48
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/ubuntu-mono-dark/apps/48$ le -a
ssh-entrypoint: le: command not found
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/ubuntu-mono-dark/apps/48$ ls -a
.  ..  .NUGGET
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/ubuntu-mono-dark/apps/48$ cat .NUGGET
Congratulations, you found the clue!
The next clue is in: /usr/lib/python3/dist-packages/py/_io/__pycache__

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/ubuntu-mono-dark/apps/48$ cd /usr/lib/python3/dist-packages/py/_io/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/py/_io/__pycache__$ ls -a
.  ..  .EVIDENCE  __init__.cpython-38.pyc  capture.cpython-38.pyc  saferepr.cpython-38.pyc  terminalwriter.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/py/_io/__pycache__$ cat .EVIDENCE
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{IotMOsMmqJ45XMiUMvV-XZMX8zw.dljM4QDLxMDO1czW}
```
## RESOURCES 
NONE
