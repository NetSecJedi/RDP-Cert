# RDP-Cert
# Manually Configure RDP to use SSL cert instead of Self-Signed

<#
	.EXAMPLE From Windows Command line (requires elevation)
			C:> powershell.exe -ExecutionPolicy Bypass -command "& { . 'RDP-Cert.ps1'; Invoke-CheckMyCerts }"
			C:> powershell.exe -ExecutionPolicy Bypass -command "& { . 'RDP-Cert.ps1'; Invoke-ImportCert }"
			C:> powershell.exe -ExecutionPolicy Bypass -command "& { . 'RDP-Cert.ps1'; Invoke-SetRDPCert }"
			C:> powershell.exe -ExecutionPolicy Bypass -command "& { . 'RDP-Cert.ps1'; Invoke-CheckRDPCert }"
			
			
	.EXAMPLE From PowerShell
			PS> . "RDP-Cert.ps1"
			PS> Invoke-CheckMyCerts
			PS> Invoke-ImportCert <password>
			PS> Invoke-SetRDPCert <num>
			PS> Invoke-CheckRDPCert
#>
