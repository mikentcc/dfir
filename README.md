# dfir on flipper zero
# I wanted to try to help with IR investigations with automating some of it trying to use a flipper zero

# Both of these payloads are for the BadUSB/BadKB module on the flipper
# Both of thses payloads do require you setup a pre-deployed server on your own

# get-velociraptor will require you setup your own Velociraptor instance and create your agent for that instance.

# get-kape will require you setup your own web server and SFTP server.  For my testing I used a Linux server with either Apache or Lighttpd web servers.

# get-velociraptor - pulls down a pre-built agent from a pre-deployed Velociraptor server.  Installs the agent and starts the service.
# You then can see the newly deployed agent in your Velociraptor server.  Then you can do your IR on the new agents/PCs

# get-kape - pulls down the Kape zip file from a pre-deployed web server then unpacks it.  It will then start a new Kape capture on the C drive 
# and run the target !SANS_Triage on the PC.  After the capture it will SFTP to a pre-deplyed SFTP server and after the transfer is completed 
# clean up the captured PC.

