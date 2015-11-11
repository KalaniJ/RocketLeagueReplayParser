# Rocket League Replay Parser

Parses replay files generated by the game Rocket League

Currently only a library. The included unit tests show some sample usage.

Completely parses all replay files. If it doesnt, please create an issue with a link to the problematic replay and I'll get it fixed up.

Network data is parsed, but it has not been completely analyzed and interpreted. For example, I know how many bits are in the data for the property "TAGame.PRI_TA:ClientLoadout", but I dont have any idea what the data means yet. But most of the interesting information has been interpreted, or it is obvious.

TODO:
* Refactor ActorStateProperties.
* Convert to JSON better. Might be easier after refactoring ActorStateProperties. By default, they dont serialize very nicely.
* Create heat maps per player/ball
* Add visualizer (preliminary tests at http://jsfiddle.net/tavay440/11/)
* Get better at actually playing Rocket League
    