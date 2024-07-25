
>[!caution] How to configure a switch in packet tracer ??
>- 1-
>	- double tab on the switch and open it.
>	- press enter to ensure you are in the CLI mode
>---
>- 2-
>	- type `enable` then enter
>	- it will appear will `#` that mean it is active and work now
>	-`show running-config` -> to show the current settings
>---
>- 3- 
>	- want to rename it ??
>		- after enable and entering the `#`
>		- `configure terminal`
>		- then `hostname {ur-name}`
>---
>- 4-
>	- wanna set password ??
>		- after enable and entering the `#`
>		- `configure terminal`
>		- `line console 0` -> outer configuration to access the switch ?
>		- `password {ur-password}`
>		- `login` ??
>---
>- 5- 
>	- wanna set an EXEC password ??
>		- after enable and entering the `#`
>		- `configure terminal`
>		- `enable password {ur-password}` -> for execution security
>---
>- 6- 
>	- wanna set a secure Exec password ??
>		- `configure terminal` or `config t`
>		- `enable secret {ur-sec-password}`
>			- this replace the old exec password with the new secret one..
>---
>- 7-
>	- verify you work ??
>		- `show run` -> or `show running-config`
>---
>- 8-
>	- encrypt the password we entered !!
>		- `config t` or `configure terminal`
>		- `service password-encryption`
>		- `exit`
>	- now it is encrypted !!
>---
>- 9-
>	- wanna set a banner !!
>		- `config t`
>		- `banner motd "what you want"`
>		- `exit`
>	- nice banner :)
>---
>- 10-
>	- now you must save your configuration by ...
>		- `enable`
>		- `copy running-config startup-config`

