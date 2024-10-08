# WhispGrid using whisper-large-v3 model
A little script to use OpenAI's [Whisper](https://github.com/openai/whisper) and is modified to use the whisper-large-v3 model https://huggingface.co/openai/whisper-large-v3 and then automatically create a TextGrid to use on [Praat](https://www.fon.hum.uva.nl/praat/). While a manual check is necessary, it saves some time. 
The app lets you choose a model from the basic OpenAI Model, or lets you enter the name of a more specific model. The language can also be chosen.

This script uses [Whisper Timestamped](https://github.com/linto-ai/whisper-timestamped) to align words and sentences, and uses two Tiers, one for segments and one for words. 
WhispGrid supports diarization based on [Riteshhere](https://github.com/riteshhere/Speaker_diarization)'s code. 

This script has been modified to detect code switches between Cantonese and English using "yue" and only began support with "whisper-large-v3".
The script "whispgrid_large_v3.py" is used for only sentence tier level transcriptions and the script "whispgrid_large_v3_words.py" is used for sentence and word tier level transcriptions.

## Functionalities

- Multiple files support
- Language Choice
- Model Choice
- Diarization (choice of number of speakers)
- Choose how diarization is displayed (initials of speakers, full name, number, etc.)
- Choose to spell out numbers or not

## Limitations

WhispGrid has a limit of 25MB per file (defined by Whisper's API).
