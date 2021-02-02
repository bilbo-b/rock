# rock
a shell script to remote control some aspects of a roonlabs ROCK installation

	rock <cmd>
	
	possible <cmd> are:
	poweroff:  shuts down gracefully and powers off at $ROCKIP
	wake:      sends "magic packet" to ROCK over network to power on
	status:    gives back some JSON-formatted status output of ROCK at $ROCKIP
	has_cdrom: outputs "no_cd_rom" if none connected or other
	eject:     ejects disk in a connected CDROM (if one is connected)
	reboot:    reboots your ROCK
	restart:   restarts ROON software
	stop:      stops ROON software 
	wake:      sends "magic packet" to ROCK over network to power on
	requirements:
	poweroff, status, has_cdrom, eject, reboot, restart, stop need "curl"
	wake needs "etherwake" and the proper mac-address in /etc/ethers for "rock"
	status, has_cdrom and eject need "jq" installed>

for more information on ROCK (roon optimized core kit) see https://help.roonlabs.com/portal/en/kb/articles/roon-optimized-core-kit
