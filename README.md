# engiword-voice

Speech recognition models for the EngiWord game, served at https://voice.engiword.com.

The archives in `vosk/` are the small Vosk models from https://alphacephei.com/vosk/models,
repacked as `.tar.gz`. They are distributed under the Apache 2.0 license.

The clips in `audio/` say the words of the game: `audio/<version>/<language>/<first letter of the
word id>/<word id>.mp3`; the clips in `audio/<version>/<language>/letters/` say the names of the
letters of the language's alphabet, each named by its code point (`10d1.mp3` is `ბ`). They were
generated with:

- Silero `v5_cis_base_nostress` (MIT, https://github.com/snakers4/silero-models): Russian
  (`ru_bogdan`) and Georgian (`kat_vika`);
- Kokoro-82M (Apache 2.0): English (`af_heart`) and Spanish (`em_santa`);
- the Piper voice `it_IT-serena-medium` (CC BY 4.0): Italian.
