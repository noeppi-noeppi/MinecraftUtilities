# Javadoc Links

Contains json files with information how to link your own javadoc to javadoc hosted somewhere else.

The json is a json object with the three keys `minecraft`, `mcp` and `forge`. Each of these is a list which contains javadoc links.

The `mcp` list should only be applied if the code for the javadoc uses MCPConfig.

The `forge` list should only be applied if the javadoc is for a forge mod.

Every entry in one of these lists is a json object. This json object always contains the key `url` which is a URL to the remote javadoc to link to. It may also contain a key `res` which is a URL to a zip or jar file containing the built javadoc. This is the case if the resource at `url` is only built on demand, and it is not possible to rely on its presence while building the javadoc.

<b>The files will change (for example before forge is released, the forge list will be empty.)</b>