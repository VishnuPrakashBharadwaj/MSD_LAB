# MSD LAB Steps:
## Connecting to the ug_vlsi_server
- Open MobaXterm. Start a new SSH session with host = 10.40.4.51, username = userx (x = 1 to 99). Password is 'student@123'.
- In case the above doesn't work, then using CLI : Connect to ug_vlsi_server using any userx (x = 1 to 99). The password is 'student@123'.
  ```console
  $ ssh -X user3@10.40.4.51
  ```
- Start a new cshell (csh) and source ~/cshrc1 or ~/cshrc_digi
  ```console
  $ csh
  $ source ~/cshrc1
  ```
- Change directory to ~/cadence_ms_labs_614
  ```console
  $ cd ~/cadence_ms_labs_614
  ```
- Start Virtuoso in the background.
  ```console
  $ which virtuoso
  /cadence_installs/IC618/bin/virtuoso
  $ virtuoso &
  ```
- Cadence Virtuoso GUI window should open.

## Creating new library
