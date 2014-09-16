steamcmd-ansible
=========

Installs the SteamCMD utility provided by Valve for downloading and installing various game servers.

Requirements
------------

This role installs the required lib32gcc1 and libc6-i386 packages. It also installs curl and libcurl3 if not already installed.

Role Variables
--------------

steamcmd_package_filename: The filename of the zip package downloadable from the Steam site
steamcmd_package_url: The url to the zip package downloadable from the Steam site
steamcmd_user: A user account to install and run SteamCMD as.

steamcmd_user_createhome: Whether to create the SteamCMD user account home directory (This can be set to no if steamcmd_path is not in the steamcmd user's home directory)
steamcmd_path: The path to install and run SteamCMD from

Dependencies
------------

n/a

Example Playbook
----------------

    - hosts: servers
      roles:
         - steamcmd

License
-------

BSD

Copyright (c) , All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

Author Information
------------------

wardavison
