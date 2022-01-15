# MCP Archive
Archive of the MCP mappings formerly hosted by MCPBot.

In modern times they are also hosted on https://maven.minecraftforge.net/. However, since Forge themselves have proven largely disinterested in maintaining the effort which was once put into creating these mappings, and since their repositories are generally unreliable, creation of such archive would appear to be a neccessessity.

### What is versions.json and real_versions.json?

The **versions.json** is the file directly copied from [Forge's Maven](https://maven.minecraftforge.net/de/oceanlabs/mcp/versions.json) and can be used by ForgeGradle 1.x/2.x as-is. It is currently used by my [ForgeGradle fork](https://github.com/juanmuscaria/ForgeGradle). The **real_versions.json** is an updated indexing that obeys the same format and contains all mappings which are actually present in the repository. In can in theory be used for the same purpose, but doing so would require additional changes in ForgeGradle itself, as it assumes no empty `snapshot`/`stable`/`snapshot_nodoc`/`stable_nodoc` entries can exist, which is not the case with last modern mappings.
