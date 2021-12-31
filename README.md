# PowerShell
Personalización para PowerShell

Pasos:

1.- Instalar terminal
2.- Instalar Powershell (La nueva version)
3.- Instalar fonts (https://www.nerdfonts.com/font-downloads)
	- Hack 
- Configurar terminal
	- Inicio
		- Perfil Predeterminado
			- Powershell (El nuevo)
	- Apariencia
		- Mostrar acrilico en fila de pestañas
			- Reiniciar terminal
	- Abrir archivo JSON
		- Buscar "schemes" -> "One Half Dark" y hacer una copia
		- Renombrarlo como "One Half Dark (modded)"
		- Cambiar el "background": "#001B26"
		- Guardar el archivo
	- Perfiles
		- Valores Predeterminados
			- Apariencia
				- Combinacion de colores
					- One Half Dark (modded)
				- Tipo de fuente
					- Hack NF
				- Acrilico
					- Activar
					- Opacidad 35%

- Instalar Scoop (ScoopInstaller)
	- Scoop is a command-line installer for Windows.
	- https://github.com/ScoopInstaller/Scoop
	- En la terminal
		iwr -useb get.scoop.sh | iex
		scoop install curl sudo jq
		curl 'https://api.inkdrop.app/' | jq
		
- Instalar Git para Windows
	- En la terminal
		winget install -e --id Git.Git

- Instalar NeoVim
	- En la terminal
		scoop install neovim gcc
	
- Crear user profile y agregar alias de comandos
	mkdir .config/powershell
	nvim .config/powershell/user_profile.ps1
		- El archivo adjunto
	cd Documents
	mkdir PowerShell
	nvim $PROFILE.CurrentUserCurrentHost
		. $env:USERPROFILE\.config\powershell\user_profile.ps1
- Instalar Oh my posh
	cd .config\powershell\
	Install-Module posh-git -Scope CurrentUser -Force
	Install-Module oh-my-posh -Scope CurrentUser -Force

- Instalar NodeJS
	scoop install nvm
	nvm install v16.13.1
	nvm use 16.13.1

- Instalar Terminal Icons
	Install-Module -Name Terminal-Icons -Repository PSGallery -Force

- Instalar z - Direcory jumper
	Install-Module -Name z -Force

- Instalar PSReadLine - Autocompletado
	Install-Module -Name PSReadLine -AllowPrerelease -Scope CurrentUser -Force -SkipPublisherCheck
- Instalar Fzf - Fuzzy finder
	scoop install fzf
        Install-Module -Name PSFzf -Scope CurrentUser -Force


