# **proxmox-lxc-scripts**

Collection of scripts adapted  and added to /usr/local/bin to run pct exec and pct push on LXC containers (including all). 

Usage:

**lxc-exec**

    lxc-exec VMID "COMMAND"

**lxc-exec-all**

    lxc-exec-all "COMMAND"

The command should be within quotations.

Example:

    lxc-exec 100 "apt install -y git"

**lxc-push**

    lxc-push VMID LOCALFILE REMOTELOCATION

    lxc-push-all LOCALFILE REMOTELOCATION

When using lxc-push REMOTELOCATION can be either a directory or a new folder and filename. For examaple /opt/ would move the file with the same name to the /opt directory in the LXC.

Example:

    lxc-push-all /opt/my_file.conf /opt/new_file_name.conf

