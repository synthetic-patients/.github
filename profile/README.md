## Synthetic Patients

![revised_group](https://github.com/synthetic-patients/.github/assets/2191507/11dc7f6a-5c68-4894-aa2c-fe30c91728a5)

[Preprint](https://google.com)
[Demo video]

### Real-time chat application

To experiment with the realtime video chat application, you will need to run it locally. We have provided a [docker container](https://hub.docker.com/r/syntheticpatients/base)  with the requirements.  You will need: API keys for OpenAI and ElevenLabs to run this program; you will be prompted to provide them. You will need an account to both of these services to get the keys and will be charged for usage. These keys will only be stored within your instance of docker and will not be shared.

To begin, make sure that you have Docker installed. Then, from your command-line, run:

```
docker pull syntheticpatients/base
```

This will take a significant amount of time to download, as it currently is around 8GB. Once this has been completed, you can run the script by executing the following in your terminal:

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/synthetic-patients/synthetic-patients-containerized/main/code/run.sh)"
```

This will launch the synthetic patient server using your OpenAI and ElevenLabs API. Once the server has completed launching, direct your browser to http://localhost:5000/client to begin interacting.

### Notes

- Because of docker's audio limitations, voice-recognition has been disabled. You will need to input text through a text field.
- Depending on the computer running the server, response times may be quite slow. 


