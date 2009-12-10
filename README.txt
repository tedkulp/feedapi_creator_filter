==================================================================================
Creator Filter
==================================================================================

Creator filter will check the <dc:creator> field of feed items against a set of
keyword(s) immidiately after parsing. Any item, that has no maching keywords will
not be saved with the feed.

IMPORTANT: The dc:creator field will only show up if the Exhaustive Parser module
is enabled, as the dc:creator field is usually not parsed into the stardard feedapi
entry.

Keywords should be sepparated by comma  e.g. "iPhone, +battery, -problem".
Keywords that start with minus (-) will be used as negative keywords.
You can also use phrases - e.g. "top performance, -bad problems".

You can use plus sign (+) in front of positive keywords if you want, but this
is not required.

If you define more than one keyword then the feed item will be included if
any of the keywords is found.

The negative keywords dominate over positive ones. So if the negative keyword is
found the feed item will be always dropped.

The search is case insensitive. The keyword 'iPhone' is just as good as the
keyword 'IPHONE' or 'iphone'.
