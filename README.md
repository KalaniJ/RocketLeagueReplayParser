# Rocket League Replay Parser
master branch: ![Build status](https://api.travis-ci.org/jjbott/RocketLeagueReplayParser.svg)

Parses replay files generated by the game Rocket League. Parses to C# objects, which can be serialized to JSON.

Supports all replay files created by Rocket League version 1.63 (released 2019-06-05) and earlier. Newer versions may work as well - updates don't always change the replay format. Changes to the replay format are usually supported within a few days. Please create an issue for any replays that fail to parse, or for replays that parse incorrectly.

Includes a library that can be used in your project (```Install-Package RocketLeagueReplayParser```) as well as a basic console based front end that can be used to convert a replay file to JSON. 

#### Example usage:

* Convert a single replay file to JSON, outputting the result to stdout

```RocketLeagueReplayParser.exe example.replay```

* Convert a single replay file to JSON, outputting the result to a file (named <file>.json)

```RocketLeagueReplayParser.exe example.replay --fileoutput```

* Convert all replay files in a directory to JSON, outputting the result to files

```RocketLeagueReplayParser.exe "\\path\to\replay\files" --fileoutput --d```

Further instructions can be found by running ```RocketLeagueReplayParser.exe --help```

#### TODO:
* Get it working under Mono (JSON serialization fails)
* Has some "Unknown" properties that I havent bothered tracking down yet.
* Code needs some cleanup. It's getting scary in there.
  
