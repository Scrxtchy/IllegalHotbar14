# [Patcher Page](https://scrxtchy.github.io/IllegalHotbar14/)

It's very barebones right now, but I want to have something that works, while perhaps an extended project in the future if more data can be mapped out efficiently

Currently, it's just looking for emote actions identified by `0x37` in the 8th byte of each entry on the hotbar, with each entry been given 8 bytes, or 64 bits. We then filter out the action IDs of these entries, specifically looking for `0x74` and `0x75` in the first byte, which correspond to Smile and Straightface respectively.

Replacing the values with some secret datamined values allow us to replace these values with `0x51` for chair sitting, and `0x69` for bed sleeping.