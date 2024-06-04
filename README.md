# MSD LAB Steps:
## Connecting to the ug_vlsi_server
- Open MobaXterm. Start a new SSH session with host = 10.40.4.51, username = userx (x = 1 to 99). The password should be provided by the lab instructor.
- In case the above doesn't work, then using CLI : Connect to ug_vlsi_server using any userx (x = 1 to 99). The password should be provided by the lab instructor.
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
- Go to File > New > Library
- Give a name to your Library.
- Under Technology File, select 'Attach to an existing technology library' and hit apply.

  ![image](https://github.com/VishnuPrakashBharadwaj/MSD_LAB/assets/39427770/1996c54f-8674-440c-8df8-3e719474e6f5)

- A new window will pop up for selecting the technology library. Select gpdk045 and hit apply. Then close both the windows.
  
  ![image](https://github.com/VishnuPrakashBharadwaj/MSD_LAB/assets/39427770/c1269490-7851-4f77-b586-45759e5e73e3)

- A success message should be shown in the console in Virtuoso GUI.
  ```
  Loaded gpdk045/libInit.il successfully!
  INFO (TECH-180011): Design library '1BM21EC209_test' successfully attached to technology library 'gpdk045'.
  INFO (TECH-180011): Design library '1BM21EC209_test' successfully attached to technology library 'gpdk045'.
  ```

## Creating a new Cellview
- Go to File > New > Cellview
- Select your newly created library and give a name to your Cellview.

  ![image](https://github.com/VishnuPrakashBharadwaj/MSD_LAB/assets/39427770/e384ea70-7adf-44cc-a60f-3548509710c0)

- Click OK to create the Cellview.
- If no problem occurs, an empty Virtuoso Schematic Editor window should open.
