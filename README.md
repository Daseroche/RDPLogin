Remote Desktop Login User Interface

Install package:
python-qt4, python-configparser, paython-urllib3

FreeRDP
sudo apt-get install freerdp -y

Configuration:
[DEFAULT]
 RDPBinary = xfreerdp
 RDPDomain = RPiTC
 RDPServer = server1.domain.lan server2.domain.lan server3.domain.lan
 RDPDomainFlags = /d:
 RDPServerFlags = /v:
 RDPUserFlags = /u:
 RDPPasswordFlags = /p:
 RDPDefaulfFlags = /cert-ignore /f +clipboard
 RDPExtraFlags = /sound:sys:alsa /rfx /fonts

 RDesktop
 sudo apt-get install rdesktop -y
 
 Configuration:
 [DEFAULT]
 RDPBinary = rdesktop
 RDPDomain = RPiTC
 RDPServer = server1.domain.lan server2.domain.lan server3.domain.lan
 RDPDomainFlags = "-d "
 RDPServerFlags = ""
 RDPUserFlags = "-u "
 RDPPasswordFlags = "-p "
 RDPDefaulfFlags = "-x l -f"
 RDPExtraFlags = "-r sound:local:alsa -z"
