# Automatizar-Backups-FTPES-Batchfile
Batchfile - Automatizar Backups FTPES con WinSCP, 7zip (2017)

recursos: Es necesario establecer como variables de entorno del sistema Windows los binarios: WinSCP.com y 7z.exe

- 1. Se establecen las variables
- 2. Se comprimen los datos en un único fichero comprimido temporal
- 3. Se envía el fichero comprimido a un servidor FTP de modo seguro
- 4. Se genera un único log de las acciones realizadas
- 5. Se envía el log por correo vía Gmail
- 6. Se eliminan los temporales creados en el proceso

backup.bat: establecer los valores deseados en las variables

- set passwd7z=passwd7z
- set pathTempFichero7z="pathTempFichero7z"
- set pathLocalDatos="pathLocalDatos"
- set pathRemotoFTP=pathRemotoFTP
- set usuarioFTP=usuarioFTP
- set passwdFTP=passwdFTP
- set servidorFTP=servidorFTP

envio_log_email.ps1: establecer los valores deseados en las variables

- $usuarioEmail = "usuarioEmail@gmail.com" 
- $passwdEmail = "passwdEmail"
- $asuntoEmail = "asuntoEmail"
- $cuerpoEmail = "cuerpoEmail"

Más info: https://www.zonasystem.com/2017/07/automatizar-copias-de-seguridad-ftps-winscp-taskschd.html
