
# gamespy-masterserver

ReadMe is incomplete and a work in progress, please open an issue if you have a question!

## Compiling
To compile a new master server

- Get the source code
  `git clone https://github.com/derkalle4/gamespy-masterserver`
  (Alternatively other folks of the project would be substituted above)
- OPTIONAL STEP FOR SWBFI/II master-server SPECIFICALLY

  Replace [ListRequestPacket.vb](./GamespyMasterserver/class/network/packets%20[tcp]/ListRequestPacket.vb) with an [older version](https://github.com/derkalle4/gamespy-masterserver/tree/81dd252320cf7950804d375990d52359717dc209)

  > latest commit has additional features
  > (namely servergroup push)
  > which appearently broke normal serverlist requests

- (VISUAL STUDIO METHOD) Open [GamespyMasterServer.sln](./GamespyMasterServer.sln)

  2017 has been used, but the SLN file states that version 10 thru 12 are targetted
 Run Build or Rebuild
 Find the built binary in /bin/debug

- (Ubuntu dotnet method)
Make sure you have `dotnet` available
You can use the snap package for the SDK version:
`sudo snap install dotnet`

 - The database schema is documented in [schema.md](./schema.md)
